# Platform Architect -> ML Engineer: Bridge Guide

**For:** Vinoth (Platform Architect at Ford) preparing for GCP Professional ML Engineer Exam
**Your strengths:** Terraform, Kubernetes, GCP infra, CI/CD (Atlantis/ArgoCD), networking, IAM, Helm, GKE, Cloud Build

This document maps every ML exam concept to something you already know. Learn faster by building on your existing mental models.

---

# SECTION 1: THE BIG PICTURE MAPPING

## Your World vs ML World

| Your World (Platform/Infra) | ML World (Exam) | Why It's the Same |
|---|---|---|
| Terraform code | ML model code (Python/TF/PyTorch) | Both are the "source" that produces the artifact |
| `terraform plan` | Model training | Both take input (code + data) and produce an artifact |
| `terraform apply` | Model deployment | Both push the artifact to production |
| `.tfstate` file | Trained model (SavedModel/pickle) | Both are the artifact that represents current state |
| Terraform state in GCS | Model in Model Registry | Both version and store the production artifact |
| `terraform.tfvars` | Training data + hyperparameters | Both are inputs that shape the output |
| Terraform modules | ML pipeline components | Both are reusable building blocks |
| Atlantis/ArgoCD | Vertex AI Pipelines | Both automate the plan->apply->verify workflow |
| Pre-commit hooks / `terraform validate` | Data validation (TFDV) | Both catch bad input before it causes damage |
| `terraform plan` diff | Model evaluation (TFMA) | Both compare "what will change" before applying |
| Sentinel/OPA policies | Model blessing (TFMA Evaluator) | Both gate deployment based on policy checks |
| Helm chart values | Hyperparameters | Both are configuration knobs that change behavior |
| GKE node pools | Training hardware (CPU/GPU/TPU) | Both are compute resources you size for the workload |
| Pod auto-scaling (HPA) | Endpoint auto-scaling | Both scale replicas based on demand |
| Container images in Artifact Registry | ML containers in Artifact Registry | Literally the same thing |
| GitOps (ArgoCD sync) | CT (Continuous Training) | Both auto-apply when source changes |
| Monitoring (Cloud Monitoring) | Model Monitoring | Both detect when production state drifts from expected |

---

# SECTION 2: CONCEPT-BY-CONCEPT BRIDGE

## 2.1 MLOps = GitOps for ML

You already live MLOps -- you just call it GitOps/IaC.

| MLOps Level | Your Equivalent | What It Means |
|---|---|---|
| **Level 0: Manual** | SSH into VM, run terraform manually | Data scientist trains in notebook, hands pickle to ops |
| **Level 1: Pipeline Automation** | Atlantis auto-running `plan`+`apply` on PR | Pipeline auto-trains model when new data arrives (CT) |
| **Level 2: CI/CD for Pipeline** | ArgoCD + Cloud Build testing Helm charts before deploy | Cloud Build tests pipeline code, auto-deploys pipeline itself |

**Your edge:** You already operate at Level 2 for infra (ArgoCD + CI/CD + Helm). The exam just wants you to know the ML version of the same thing.

---

## 2.2 Vertex AI Pipelines = Atlantis for ML

| Atlantis Concept | Vertex AI Pipelines Equivalent |
|---|---|
| `atlantis.yaml` (workflow definition) | Pipeline definition (Kubeflow SDK / TFX) |
| Workspace variables | Pipeline parameters (hyperparameters, data paths) |
| `plan` step | Data validation + preprocessing steps |
| `apply` step | Training step |
| Plan output review | Model evaluation (TFMA) |
| Apply approval gate | Model blessing (Evaluator threshold check) |
| Post-apply hooks | Model deployment to endpoint |
| Lock per workspace | One pipeline run per experiment |
| repos.yaml routing | Pipeline triggers (Cloud Scheduler, Eventarc) |

**Key insight for exam:** When you see "automate ML workflow end-to-end" -> think "this is Atlantis but for models, not Terraform."

---

## 2.3 Feature Store = Terraform State Backend

| Terraform State | Feature Store |
|---|---|
| Single source of truth for resource state | Single source of truth for feature values |
| Remote backend (GCS) prevents local drift | Feature Store prevents training-serving skew |
| State locking prevents concurrent corruption | Point-in-time lookups prevent data leakage |
| Multiple workspaces read same state | Multiple models read same features |
| `terraform output` for downstream use | Online serving for real-time prediction |
| `terraform state pull` for inspection | Offline serving for batch training |

**Key insight for exam:** Training-serving skew = the ML version of "someone ran terraform locally and now state is out of sync." Feature Store = the ML version of "put your state in GCS remote backend so everyone uses the same truth."

---

## 2.4 Model Monitoring = Drift Detection (Like State Drift)

| Infra Drift | ML Drift | Detection |
|---|---|---|
| `terraform plan` shows unexpected changes | **Data drift**: input features shifted | Compare serving distributions vs training baseline |
| Infrastructure config changed outside Terraform | **Training-serving skew**: features computed differently | Compare feature computation paths |
| Requirements changed but code didn't update | **Concept drift**: world changed, model didn't | Performance metrics declining over time |
| Helm values don't match running state | **Prediction drift**: output distribution shifted | Monitor prediction patterns |
| Someone `kubectl apply`-ed directly | **Feature attribution drift**: what matters changed | Feature importance shifting |

**Your mapping cheat:**

| If you see this keyword... | Think of this infra problem... | ML answer is... |
|---|---|---|
| "Training-serving skew" | State drift (local vs remote tfstate) | Feature Store or tf.Transform |
| "Data drift" | Input parameters changed | Vertex AI Model Monitoring |
| "Concept drift" | Requirements changed, code is stale | Retrain the model |
| "Prediction drift" | Outputs changed unexpectedly | Monitor + investigate |

---

## 2.5 Containers & Serving = You Already Know This

You deploy workloads on GKE daily. ML serving is the same thing.

| GKE Concept | ML Serving Equivalent |
|---|---|
| Deployment + Service | Vertex AI Endpoint |
| Pod replicas | Endpoint replicas (min/max) |
| HPA (Horizontal Pod Autoscaler) | Endpoint auto-scaling |
| Container image from Artifact Registry | Pre-built or custom prediction container |
| Rolling update (maxSurge, maxUnavailable) | Traffic splitting / canary deployment |
| Blue-green deployment | A/B testing between model versions |
| NodePort / ClusterIP / LoadBalancer | Public vs private endpoints |
| Resource requests/limits (CPU/memory) | Machine type + GPU selection |
| Anti-affinity rules | Multi-region deployment |
| Liveness/readiness probes | InfraValidator (TFX) |
| Namespace isolation | VPC Service Controls |
| Network policies | Private endpoints + VPC peering |

**Key insight for exam:** When you see "deploy model to production" -> think "this is just deploying a container to GKE but Google manages the cluster for you (Vertex AI Endpoints)."

### Container Selection (You Already Understand This)

| Helm Chart Analogy | ML Container Decision |
|---|---|
| Official Helm chart from ArtifactHub | **Pre-built container** (TF, PyTorch, sklearn, XGBoost) |
| Custom Helm chart with your own templates | **Custom container** (your Dockerfile, any framework) |
| When to use official: standard app, no special needs | When to use pre-built: standard framework, no special deps |
| When to use custom: special config, custom sidecars | When to use custom: CatBoost, custom preprocessing, special libs |

---

## 2.6 Distributed Training = Node Pool Scaling

You scale GKE node pools for workloads. ML training scales similarly.

| GKE Scaling | ML Training Strategy | When |
|---|---|---|
| Single node, add CPU/memory | Single machine, bigger GPU | Model fits, just need more power |
| Single node, add GPUs (multi-GPU node pool) | **MirroredStrategy** | Model fits in 1 GPU, data is large |
| Multi-node cluster (multiple nodes) | **MultiWorkerMirroredStrategy** | Need >8 GPUs (max per machine) |
| Pod sharding (split app across pods) | **Model parallelism** | Model too large for 1 GPU memory |
| Data sharding (split data across replicas) | **Data parallelism** | Same model, different data chunks |

**Your mental model:**
- `MirroredStrategy` = single node with multiple GPUs = like a single GKE node with multiple CPUs
- `MultiWorkerMirroredStrategy` = multi-node = like scaling your node pool across machines
- `Model parallelism` = sharding a stateful app across pods = model split across GPUs
- `Data parallelism` = stateless app replicas = same model on each GPU, different data

---

## 2.7 CI/CD for ML = Your Cloud Build / ArgoCD Knowledge

| Your CI/CD Stack | ML CI/CD Equivalent |
|---|---|
| Cloud Build triggers on MR | Cloud Build triggers on pipeline code change |
| Build step: `terraform validate` | Build step: unit test pipeline components |
| Build step: `terraform plan` | Build step: run pipeline on test data |
| Build step: push to Artifact Registry | Build step: push training container to Artifact Registry |
| ArgoCD syncs desired state to cluster | Vertex AI Pipelines deploys trained model to endpoint |
| ArgoCD health checks | Model evaluation + blessing |
| ArgoCD rollback | Traffic split rollback to previous model version |

---

## 2.8 Data Processing = Your ETL Knowledge

You've worked with data pipelines. Here's the ML mapping:

| What You Know | ML Equivalent | Exam Service |
|---|---|---|
| Cloud SQL -> BigQuery ETL | Training data preparation | **Dataflow** (streaming+batch) |
| Scheduled BigQuery queries | Batch feature computation | **BigQuery** scheduled queries |
| Pub/Sub event processing | Real-time feature computation | **Dataflow** streaming |
| Apache Spark on Dataproc | Large-scale data processing | **Dataproc** (existing Spark code) |
| Terraform variable precedence | Feature engineering (transforms) | **tf.Transform** / Feature Store |

### The Processing Service Decision (in your language)

| If This Were Infra, You'd Use... | For ML, Use... | Because |
|---|---|---|
| Cloud Functions (event-driven, small) | Cloud Functions | Simple triggers, light processing |
| GKE CronJob (scheduled, medium) | Cloud Scheduler + Vertex AI Pipeline | Scheduled training runs |
| Dataflow (streaming, serverless) | **Dataflow** | Streaming features, exactly-once |
| Dataproc (you have Spark code) | **Dataproc** | Existing PySpark feature engineering |
| BigQuery (SQL transforms) | **BigQuery** | SQL-based feature engineering |
| Cloud Composer (complex DAG) | **Cloud Composer** | Complex multi-source orchestration |

---

## 2.9 Security & IAM = Your Strongest Area

You manage IAM, VPC, firewalls, SA impersonation daily. ML security is IDENTICAL.

| Your Daily Work | ML Exam Equivalent |
|---|---|
| Service Account impersonation (Atlantis -> per-env SA) | Training/serving SA with minimal permissions |
| VPC Service Controls perimeter | Prevent training data exfiltration |
| CMEK for GCS/BigQuery | Encrypt model artifacts with org keys |
| Private GKE clusters (no public endpoint) | Private Vertex AI endpoints (VPC peering) |
| Firewall rules (ingress/egress) | Network policies for endpoints |
| Shared VPC / host-service project | Vertex AI in service project accessing data in host project |
| IAM deny policies | Prevent unauthorized model access |
| Audit Logs | Prediction request/response logging |
| Cloud Armor WAF | Model Armor (for Gen AI prompt safety) |

**Key insight:** When the exam asks about ML security, it's the SAME GCP security stack you already know. The only new concept is **Model Armor** (inspects LLM inputs/outputs for safety).

---

# SECTION 3: THE HARD PARTS (Where Your Background Doesn't Help)

These are the topics with NO infra equivalent. Focus extra study time here.

## 3.1 ML Fundamentals You Must Learn Fresh

| Topic | What to Know | Exam Focus |
|---|---|---|
| **Overfitting vs Underfitting** | Overfit = memorizes training data (low train loss, high val loss). Underfit = model too simple (both losses high). | Diagnosing training issues from loss curves |
| **Bias-Variance Tradeoff** | High bias = underfit. High variance = overfit. Balance with model complexity + regularization. | "Model plateaus at 72%" = underfitting |
| **Evaluation Metrics** | Accuracy, Precision, Recall, F1, AUC-ROC, AUC-PR. NEVER use accuracy alone on imbalanced data. | "Minimize false negatives" = recall |
| **Class Imbalance** | 98:2 ratio -> accuracy is meaningless (predicting majority always = 98%). Use F1, AUC-PR, SMOTE, class weights. | Medical/fraud data questions |
| **Train/Val/Test Splits** | Random for i.i.d. data. TIME-BASED for temporal data (train on past, test on future). Stratified for imbalanced. | Temporal data leakage trap |
| **Regularization** | L1 (sparse features), L2 (prevent large weights), Dropout (neural nets). Prevents overfitting. | "Model overfitting" -> add regularization |
| **Transfer Learning** | Start with pre-trained model, fine-tune on your data. Works with limited data. | "Only 200 labeled images" -> transfer learning |

### Quick Mental Models for ML Metrics

Think of it like monitoring:

| ML Metric | Monitoring Analogy |
|---|---|
| **Accuracy** | Overall uptime % (misleading if you only count healthy pods) |
| **Precision** | "Of all alerts fired, how many were real incidents?" (false alarm rate) |
| **Recall** | "Of all real incidents, how many did we detect?" (miss rate) |
| **F1 Score** | Harmonic mean of precision + recall (balanced score) |
| **AUC-ROC** | "How well does our alerting system separate real incidents from noise across all thresholds?" |

**The exam LOVES this scenario:**
> "Your fraud detection model has 99% accuracy on data where 1% of transactions are fraudulent."
> **Translation:** "Your monitoring shows 99% uptime but only because you're not counting the 1% of critical failures." -> Accuracy is meaningless. Use precision/recall.

---

## 3.2 Model Types Decision Tree (No Infra Equivalent)

You need to memorize WHEN to pick each model type:

```
What's your data?
├── Structured/Tabular
│   ├── Predict a category? -> Classification (logistic regression, XGBoost, DNN)
│   ├── Predict a number? -> Regression (linear regression, XGBoost, DNN)
│   ├── Find groups (no labels)? -> Clustering (K-means)
│   ├── Find outliers (no labels)? -> Anomaly detection (autoencoder, isolation forest)
│   └── Predict future values? -> Time series (ARIMA, LSTM, Prophet)
│
├── Images
│   ├── Classify images? -> Image classification (CNN, ResNet, AutoML Vision)
│   ├── Find objects in images? -> Object detection (YOLO, AutoML)
│   └── Segment images? -> Semantic segmentation (U-Net)
│
├── Text
│   ├── Classify text? -> Text classification (BERT, AutoML Text)
│   ├── Extract entities? -> NER (BERT, Natural Language API)
│   ├── Generate text? -> LLM (Gemini, fine-tuned foundation model)
│   └── Translate? -> Translation (Translation API, seq2seq)
│
└── Recommendations -> Collaborative filtering (matrix factorization, BQML)
```

---

## 3.3 Explainability Methods (No Infra Equivalent)

| Method | Works On | How It Works | Exam Keyword |
|---|---|---|---|
| **Sampled Shapley** | ANY model (black box) | Tests "what if I remove this feature?" | "tabular", "XGBoost", "random forest", "any model" |
| **Integrated Gradients** | Neural networks only | Follows the gradient path from baseline to input | "neural network", "DNN", "deep learning" |
| **XRAI** | Image models only | Groups pixels into meaningful regions | "image", "which region", "visual explanation" |

**Memory trick:** 
- **S**hapley = **S**afe for anything (universal)
- **I**ntegrated Gradients = needs **I**nternal access (gradients = neural nets only)
- **X**RAI = e**X**plains images (regions)

---

## 3.4 Hyperparameter Tuning (Partial Infra Parallel)

Think of it like tuning Helm chart values:

| Helm Tuning | HP Tuning |
|---|---|
| `replicaCount: 3` (you know the right value) | Grid search (try specific values) |
| "Try random values in a range" | Random search |
| "Use Prometheus metrics to auto-tune" | **Bayesian optimization (Vizier)** -- learns from past trials |
| "Kill pods that are clearly failing" | **Early stopping** -- kill trials performing below median |

**Exam answer is almost always: Bayesian optimization (Vizier)** because:
- It's the smartest (learns from previous trials)
- It's the most efficient (finds good values with fewer trials)
- It's the Google-managed service

---

# SECTION 4: EXAM PATTERN RECOGNITION (Your Shortcut)

After reviewing 93 questions, here are the PATTERNS the exam uses. Spot these and you'll know the answer in 10 seconds.

## Pattern 1: "Team Profile -> Service Selection"

| If the question says... | The answer is always... |
|---|---|
| "Team knows SQL, no Python" | **BigQuery ML** |
| "No ML expertise on the team" | **AutoML** or **Pre-built APIs** |
| "Data scientist with Python/TF code" | **Custom Training** |
| "Non-technical business user" | **AutoML** or **Pre-built APIs** or **BigQuery ML** |

## Pattern 2: "Minimize X -> Service Selection"

| If the question says... | The answer is always... |
|---|---|
| "Minimize operational overhead" | Most managed/serverless option |
| "Minimize cost" | Spot VMs, batch prediction, right-sizing, scale-to-zero |
| "Minimize latency" | Online prediction + GPU + Feature Store online serving |
| "Minimize code changes" | Service closest to existing code |
| "Minimize development time" | AutoML or BigQuery ML or pre-built APIs |

## Pattern 3: "Symptom -> Diagnosis"

| If the question describes... | The answer is... |
|---|---|
| "Accuracy high in eval, low in production, same data source" | **Training-serving skew** |
| "Accuracy declining over months, no code changes, features look same" | **Concept drift** |
| "Feature distributions changed between training and serving data" | **Data drift** |
| "Training loss drops, validation loss rises" | **Overfitting** |
| "Both training and validation loss plateau at same level" | **Underfitting** |
| "OOM error during training" | **Reduce batch size** |
| "98% accuracy on 98:2 imbalanced data" | **Meaningless -- use precision/recall/F1** |
| "High test accuracy, low production accuracy, temporal data" | **Data leakage from random split** |

## Pattern 4: "Scale Problem -> Distributed Strategy"

| If the question says... | The answer is... |
|---|---|
| "Model fits in 1 GPU, training slow" | **MirroredStrategy** (multi-GPU, single machine) |
| "Need >8 GPUs" | **MultiWorkerMirroredStrategy** (multi-machine) |
| "Model too large for 1 GPU memory" | **Model parallelism** |
| "Large dataset, standard model" | **Data parallelism** |
| "TensorFlow + very large scale" | **TPU** |
| "PyTorch" | **GPU** (not TPU) |

## Pattern 5: "Security Requirement -> GCP Service"

This is your STRONGEST area. Trust your instincts.

| Requirement | Service (you already know these!) |
|---|---|
| "Data can't leave the project" | VPC Service Controls |
| "Encrypt with our keys" | CMEK |
| "Only accessible from VPC" | Private endpoint with VPC peering |
| "Audit all access" | Cloud Audit Logs + prediction logging |
| "Prevent prompt injection" | Model Armor |
| "Control who accesses what" | IAM |

---

# SECTION 5: YOUR 17-DAY PRIORITY MAP

Given your platform architect background, here's what to focus your limited time on:

## SKIP (You Already Know These) -- Save 3+ Hours
- [x] GCP IAM, VPC, networking, security -- you live this daily
- [x] Container concepts (build, push, deploy, scale) -- GKE expert
- [x] CI/CD concepts (Cloud Build, Artifact Registry) -- your daily work
- [x] Infrastructure scaling, auto-scaling -- HPA, node pools
- [x] Cloud Monitoring, alerting -- already set up for Atlantis

## SKIM (Familiar Concepts, New Names) -- 2-3 Hours
- [ ] Vertex AI Pipelines -- "Atlantis for ML" (know the components)
- [ ] Feature Store -- "Remote state backend for features" (know online vs offline)
- [ ] Model Registry -- "Artifact Registry for models" (know versioning)
- [ ] MLOps levels -- "GitOps maturity for ML" (know 0/1/2)
- [ ] Model deployment -- "GKE deployment for models" (know online vs batch, traffic splitting)

## STUDY HARD (New Concepts) -- 8-10 Hours
- [ ] **Evaluation metrics** -- precision, recall, F1, AUC, class imbalance (NO infra equivalent)
- [ ] **Overfitting vs underfitting** -- loss curve diagnosis (NO infra equivalent)
- [ ] **Drift types** -- concept vs data vs skew vs attribution (partial infra parallel)
- [ ] **Explainability** -- Shapley vs Integrated Gradients vs XRAI (NO infra equivalent)
- [ ] **Model type selection** -- when to pick ARIMA vs XGBoost vs DNN vs LLM (NO infra equivalent)
- [ ] **Distributed training** -- MirroredStrategy vs MultiWorker vs model parallelism (partial parallel)
- [ ] **TFX component order** -- memorize the 10 components (NO infra equivalent)
- [ ] **BigQuery ML vs AutoML vs Custom Training** decision tree (NEW)
- [ ] **Dataflow vs Dataproc** decision criteria (you know both but not the ML decision rules)
- [ ] **Hyperparameter tuning** -- Bayesian vs grid vs random (partial parallel)

## PRACTICE (Apply Knowledge) -- 4-5 Hours
- [ ] All 93 questions in STUDY_GUIDE.md -- focus on the ones you get WRONG
- [ ] ExamTopics or Whizlabs -- 100+ additional questions
- [ ] Google's official sample questions

---

# SECTION 6: ONE-PAGE EXAM CHEAT SHEET (Print This)

```
TEAM PROFILE -> SERVICE
  SQL team         -> BigQuery ML
  No ML expertise  -> AutoML / Pre-built APIs  
  Python/TF code   -> Custom Training
  
MINIMIZE OVERHEAD -> MOST MANAGED
  Training    -> AutoML / BQML
  Serving     -> Vertex AI Endpoints
  Pipeline    -> Vertex AI Pipelines
  Processing  -> Dataflow / BigQuery

DRIFT DIAGNOSIS
  Features same + accuracy drops = CONCEPT drift -> retrain
  Feature distributions shifted   = DATA drift -> monitor + retrain
  Different preprocessing paths   = TRAINING-SERVING SKEW -> Feature Store / tf.Transform
  
DISTRIBUTED TRAINING
  1 machine, multi-GPU    = MirroredStrategy
  Multi-machine            = MultiWorkerMirroredStrategy  
  Model doesn't fit 1 GPU = Model parallelism
  TF + huge scale          = TPU

METRICS (IMBALANCED DATA)
  "Minimize false negatives" = optimize RECALL
  "Minimize false positives" = optimize PRECISION
  98% accuracy on 98:2 data  = MEANINGLESS

EXPLAINABILITY
  Any model    = Sampled Shapley
  Neural net   = Integrated Gradients
  Image        = XRAI

TFX ORDER
  ExampleGen -> StatisticsGen -> SchemaGen -> ExampleValidator 
  -> Transform -> Trainer -> Tuner -> Evaluator -> Pusher

MLOPS LEVELS
  0 = manual | 1 = automated pipeline (CT) | 2 = CI/CD for pipeline code
```

---

**Bottom line:** Your platform architect experience covers ~40% of the exam topics already. Focus your 17 days on the ~60% that's pure ML (metrics, model types, drift, explainability, TFX). The bridge mappings above will help you learn faster by connecting new concepts to things you already understand deeply.

**You've got this.**
