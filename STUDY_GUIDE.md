# Google Cloud Professional Machine Learning Engineer - Complete Exam Preparation Guide

**Exam:** PR000269 | **Date:** Monday, September 21, 2026, 4:00 PM IST | **Duration:** 135 minutes
**Location:** MINSWAY SOLUTIONS PRIVATE LIMITED
**Questions:** 50-60 multiple choice and multiple select | **Passing:** ~70% (estimated)
**Fee:** $200 | **No direct coding** but may include Python/SQL snippets to interpret

---

# TABLE OF CONTENTS

1. [Exam Domain Breakdown & Weightage](#part-1-exam-domains--weightage)
2. [Study Plan (17 Days)](#part-2-17-day-study-plan)
3. [Study Resources](#part-3-study-resources)
4. [Cheat Sheets & Decision Trees](#part-4-cheat-sheets--decision-trees)
5. [Practice Questions - Domain 1: Low-Code AI Solutions](#part-5-domain-1-architecting-low-code-ai-solutions-13)
6. [Practice Questions - Domain 2: Data & Model Management](#part-6-domain-2-collaborating-to-manage-data-and-models-16)
7. [Practice Questions - Domain 3: Scaling Prototypes](#part-7-domain-3-scaling-prototypes-into-ml-models-21---largest)
8. [Practice Questions - Domain 4: Serving & Scaling Models](#part-8-domain-4-serving-and-scaling-models-20)
9. [Practice Questions - Domain 5: ML Pipelines](#part-9-domain-5-automating-and-orchestrating-ml-pipelines-18)
10. [Practice Questions - Domain 6: Monitoring AI Solutions](#part-10-domain-6-monitoring-ai-solutions-13)
11. [Cross-Domain Gotcha Questions](#part-11-cross-domain-gotcha-questions)
12. [Top 10 Exam Failure Areas](#part-12-top-10-exam-failure-areas)

---

# PART 1: EXAM DOMAINS & WEIGHTAGE

| Section | Weight | Key Focus |
|---------|--------|-----------|
| 1. Architecting Low-Code AI Solutions | ~13% | BigQuery ML, AutoML, Pre-built APIs, Model Garden, Gemini |
| 2. Collaborating to Manage Data & Models | ~16% | Data preprocessing, Feature Store, Notebooks, Experiments |
| 3. Scaling Prototypes into ML Models | **~21%** | Custom Training, Distributed Training, GPU/TPU, HP Tuning |
| 4. Serving and Scaling Models | ~20% | Online/Batch prediction, Deployment, Traffic splitting |
| 5. Automating & Orchestrating ML Pipelines | ~18% | Vertex AI Pipelines, TFX, CI/CD, MLOps levels |
| 6. Monitoring AI Solutions | ~13% | Drift detection, Explainability, Responsible AI, Security |

**CRITICAL:** Sections 3+4 = **41% of the exam**. Master these first.

### Detailed Domain Breakdown (June 2026 Exam Guide)

**Section 1: Architecting Low-Code AI Solutions (~13%)**
- 1.1 BigQuery ML / AutoML on Gemini Enterprise Agent Platform
- 1.2 Google Cloud AI APIs / foundational models (Model Garden, Document AI, Vision API, Translate API)
- Building/tuning: Gemini, Imagen, Veo
- Optimizing Gemini apps for cost, latency, availability

**Section 2: Collaborating to Manage Data and Models (~16%)**
- 2.1 Exploring/preprocessing data (BigQuery SQL, Dataflow, Spark, Python, Feature Store, PII/privacy)
- 2.2 Model prototyping in notebooks (Workbench, Colab Enterprise)
- 2.3 Tracking/running experiments (Vertex AI Experiments, Pipelines, ML Metadata)

**Section 3: Scaling Prototypes into ML Models (~21%)**
- 3.1 Building models (model type selection, product selection, deployment strategy)
- 3.2 Training models (data organization, training SDKs, HP tuning, fine-tuning foundation models)
- 3.3 Hardware selection (CPU vs GPU vs TPU, distributed training strategies)

**Section 4: Serving and Scaling Models (~20%)**
- 4.1 Serving models (batch/online, containers, Model Registry, A/B testing, canary)
- 4.2 Scaling online serving (Feature Store, endpoints, hardware, auto-scaling)

**Section 5: Automating and Orchestrating ML Pipelines (~18%)**
- 5.1 End-to-end pipelines (data/model validation, orchestration, consistent preprocessing)
- 5.2 Automating retraining (CI/CD/CT, Cloud Build)

**Section 6: Monitoring AI Solutions (~13%)**
- 6.1 Identifying risks (security, Model Armor, Responsible AI, explainability)
- 6.2 Monitoring/testing/troubleshooting (Model Monitoring, drift detection, Gen AI evaluation)

> **Note:** The exam was updated June 2026. "Vertex AI" is now called "Gemini Enterprise Agent Platform" in some places. Both terms refer to the same services.

---

# PART 2: 17-DAY STUDY PLAN

| Period | Days | Focus (% of exam) | What to Study |
|--------|------|--------------------|---------------|
| **Week 1** | Sep 4-10 | Sections 3+4 (41%) | Training, serving, scaling, distributed training, GPU/TPU, deployment patterns |
| **Week 2** | Sep 11-17 | Sections 2+5 (34%) | Data management, Feature Store, pipelines, MLOps, TFX, CI/CD |
| **Week 3** | Sep 18-21 | Sections 1+6 (26%) + Review | Low-code AI, monitoring, drift, explainability, practice tests, weak areas |

### Daily Schedule (1-2 hours/day)
- **30 min:** Read concepts/cheat sheets
- **30 min:** Practice questions with explanations
- **30 min:** Review wrong answers, understand WHY

### Last Day Before Exam (Sep 20)
1. Review all 6 Cheat Sheets (30 min)
2. Re-do only the questions you got wrong (30 min)
3. Review the "Top 10 Failure Areas" section (15 min)
4. REST. Don't cram. Trust your preparation.

---

# PART 3: STUDY RESOURCES

### Official (FREE)
1. **Official Exam Guide PDF:** https://services.google.com/fh/files/misc/professional_machine_learning_engineer_exam_guide_english_new.pdf
2. **Official Sample Questions:** https://docs.google.com/forms/d/e/1FAIpQLSeYmkCANE81qSBqLW0g2X7RoskBX9yGYQu-m1TtsjMvHabGqg/viewform
3. **Cloud Skills Boost ML Path:** https://www.skills.google/paths/17
4. **ML Crash Course:** https://developers.google.com/machine-learning/crash-course

### Third-Party Practice Questions
1. **ExamTopics** - Large community question bank with discussion
2. **Whizlabs** - Dedicated practice exams
3. **Udemy** - Search "Google Cloud ML Engineer practice tests" (200-300 question sets)
4. **TutorialsDojo** - High-quality GCP practice exams

### Community Resources
- **GitHub:** https://github.com/sathishvj/awesome-gcp-certifications/blob/master/professional-machine-learning-engineer.md
- **Books:** "Machine Learning Design Patterns" (Lakshmanan, Robinson, Munn)
- **Books:** "Official Google Cloud Certified Professional ML Engineer Study Guide" (Wiley)

### Coursera (Priority Order)
1. ML Pipelines on Google Cloud
2. MLOps Specialization (4 courses)
3. TensorFlow Developer Specialization

### YouTube
- **Priyanka Vergadia** - "Vertex AI - AI Simplified" series
- **Google Cloud** - "AI Adventures" series
- **StatQuest (Josh Starmer)** - ROC/AUC and ML fundamentals

---

# PART 4: CHEAT SHEETS & DECISION TREES

## CHEAT SHEET 1: "Which GCP Service?" Decision Tree

### Data Preprocessing

| When you see... | Pick | Because |
|---|---|---|
| "Streaming data" or "real-time processing" or "windowing" | **Dataflow** | Apache Beam, serverless, exactly-once |
| "Same code for batch and streaming" | **Dataflow** | Beam's unified programming model |
| "Existing Spark/Hadoop code" or "PySpark" | **Dataproc** | Managed Spark/Hadoop, lift-and-shift |
| "SQL-based transforms on structured data" | **BigQuery** | Serverless, petabyte-scale |
| "Non-technical user" or "visual data wrangling" | **Dataprep (Trifacta)** | UI-based, auto-generates Dataflow jobs |
| "Enterprise ETL" or "visual pipeline builder" | **Cloud Data Fusion** | Code-free ETL, 150+ connectors |

### Model Training

| When you see... | Pick | Because |
|---|---|---|
| "Data in BigQuery" + "team knows SQL" + "quick prototype" | **BigQuery ML** | No data export, SQL interface |
| "No ML expertise" + "image/text/tabular/video" | **AutoML** | Automated architecture search, minimal code |
| "Custom architecture" or "custom loss function" or "full control" | **Custom Training** | Bring your own code, any framework |
| "Extract entities/sentiment" + "no training needed" | **Pre-built APIs** | Ready to use, pay per call |
| "Time series forecasting" + "SQL team" | **BigQuery ML (ARIMA_PLUS)** | Built-in ARIMA, no code needed |
| "Need GPUs/TPUs for training" | **Custom Training** | Only custom training gives hardware control |

### Pipeline Orchestration

| When you see... | Pick | Because |
|---|---|---|
| "Serverless ML pipeline" or "minimal ops" | **Vertex AI Pipelines** | No cluster management, built-in ML metadata |
| "TensorFlow ecosystem" + "data validation" | **TFX** | End-to-end TF pipeline with TFDV, TFMA |
| "Framework-agnostic" + "already have GKE" | **Kubeflow Pipelines** | Runs on K8s, supports any framework |
| "Complex DAG scheduling" + "non-ML tasks" | **Cloud Composer (Airflow)** | General-purpose workflow orchestration |
| "Track experiments and compare runs" | **Vertex AI Experiments** | Experiment tracking with metrics comparison |

### Model Serving

| When you see... | Pick | Because |
|---|---|---|
| "Real-time" or "low-latency" or "< 100ms" | **Online Prediction (Vertex AI Endpoints)** | Always-on, auto-scaling, GPU support |
| "Large volume" + "not time-sensitive" or "nightly" | **Batch Prediction** | Cost-effective, processes GCS/BQ data |
| "Custom serving logic" or "non-standard framework" | **Custom container on Vertex AI** | Full control over serving code |
| "Scale to zero" + "HTTP" | **Cloud Run** | Serverless containers, pay-per-request |
| "Edge deployment" or "IoT" | **Edge Manager / TF Lite** | On-device inference |

### Feature Management

| When you see... | Pick | Because |
|---|---|---|
| "Consistent features training and serving" | **Feature Store** or **tf.Transform** | Both prevent training-serving skew |
| "Reuse features across teams/models" | **Feature Store** | Centralized, discoverable, shared |
| "TensorFlow-specific preprocessing" | **tf.Transform** | Generates a TF graph applied at serving |
| "Real-time feature lookup at serving" | **Feature Store (online serving)** | Low-latency key-value lookups |

### Gen AI

| When you see... | Pick | Because |
|---|---|---|
| "Try/test prompts interactively" | **Vertex AI Studio** | UI for prompt design, testing |
| "Browse/deploy pre-trained models" | **Model Garden** | Catalog of first/third-party models |
| "Adapt model to domain data" | **Fine-tuning** | Better accuracy for specific tasks |
| "Use enterprise data without retraining" | **RAG** | Grounds responses in your data |

---

## CHEAT SHEET 2: Confusing Pairs

| Pair | Key Difference | Exam Keyword to Pick |
|---|---|---|
| **Dataflow vs Dataproc** | Dataflow = serverless Beam (streaming+batch); Dataproc = managed Spark (existing code) | "streaming"/"exactly-once" -> Dataflow; "Spark"/"Hadoop" -> Dataproc |
| **TFDV vs TFMA** | TFDV = **data** validation; TFMA = **model** analysis | "data quality/schema" -> TFDV; "model evaluation/sliced metrics" -> TFMA |
| **Data drift vs Concept drift** | Data drift = input distributions change; Concept drift = input->output relationship changes | "feature distributions shifted" -> Data drift; "accuracy drops, data looks same" -> Concept drift |
| **Data drift vs Training-serving skew** | Data drift = distributions change over *time*; Skew = features computed *differently* | "over time/gradual" -> Data drift; "different code paths" -> Skew |
| **MirroredStrategy vs MultiWorkerMirroredStrategy** | Mirrored = 1 machine, multi-GPU; MultiWorker = multi-machine, multi-GPU | "single node multi-GPU" -> Mirrored; "multi-node cluster" -> MultiWorker |
| **Data parallelism vs Model parallelism** | Data = same model, different data shards; Model = model split across devices | "large dataset" -> Data; "model too large for one GPU" -> Model |
| **Sampled Shapley vs Integrated Gradients vs XRAI** | Shapley = any model; IntGrad = neural nets; XRAI = images | "tabular/any model" -> Shapley; "neural network" -> IntGrad; "image regions" -> XRAI |
| **Online vs Batch prediction** | Online = real-time; Batch = large volume, async | "real-time/low-latency" -> Online; "nightly/bulk" -> Batch |
| **Pre-built vs Custom container** | Pre-built = Google-provided (TF/PyTorch/sklearn/XGBoost); Custom = your Docker | "standard framework" -> Pre-built; "custom dependencies" -> Custom |
| **AutoML vs BigQuery ML** | AutoML = any data type, no code, NAS; BQML = SQL, data stays in BQ | "no expertise + images/text" -> AutoML; "SQL team + structured" -> BQML |
| **Feature Store online vs offline** | Online = low-latency serving; Offline = batch training export | "real-time serving" -> Online; "training export" -> Offline |
| **VPC Service Controls vs IAM** | VPC-SC = network perimeter (prevent exfiltration); IAM = identity access | "data exfiltration" -> VPC-SC; "who can access what" -> IAM |

---

## CHEAT SHEET 3: Key Numbers & Thresholds

### CPU vs GPU vs TPU

| Choose | When |
|---|---|
| **CPU** | Small models, tabular data, sklearn/XGBoost, simple inference |
| **GPU** | Medium-large DNNs, vision, NLP, custom TF/PyTorch, transfer learning |
| **TPU** | Very large models, massive datasets, TensorFlow-only, matrix-heavy |

> **Exam tip:** "TensorFlow" + "very large scale" -> TPU. "PyTorch" -> GPU.

### MLOps Maturity Levels

| Level | Name | What it adds |
|---|---|---|
| **Level 0** | Manual | Manual training, manual deployment, no pipeline, no monitoring |
| **Level 1** | ML Pipeline Automation | Automated training pipeline, CT (Continuous Training), Feature Store |
| **Level 2** | CI/CD Pipeline Automation | Automated testing + deployment, A/B testing, full CI/CD. CT + CI + CD |

> **Exam tip:** "Automate retraining" = Level 1. "Automate testing AND deployment" = Level 2.

### TFX Component Order (MEMORIZE THIS!)

```
ExampleGen -> StatisticsGen -> SchemaGen -> ExampleValidator -> Transform -> Trainer -> Tuner -> Evaluator -> InfraValidator -> Pusher
```

| Component | Purpose |
|---|---|
| **ExampleGen** | Ingest and split data |
| **StatisticsGen** | Compute data statistics |
| **SchemaGen** | Infer data schema |
| **ExampleValidator** | Detect data anomalies (uses TFDV) |
| **Transform** | Feature engineering (uses tf.Transform) |
| **Trainer** | Train the model |
| **Tuner** | Hyperparameter tuning |
| **Evaluator** | Evaluate model quality (uses TFMA) |
| **InfraValidator** | Validate model can be served |
| **Pusher** | Deploy model to serving |

---

## CHEAT SHEET 4: "Minimize Operational Overhead" Translation Guide

| Exam phrase | Answer pattern |
|---|---|
| "Minimize operational overhead" + training | -> **AutoML** or **BigQuery ML** (serverless) |
| "Minimize operational overhead" + serving | -> **Vertex AI Endpoints** (managed, auto-scaling) |
| "Minimize operational overhead" + pipeline | -> **Vertex AI Pipelines** (serverless) |
| "Minimize operational overhead" + preprocessing | -> **Dataflow** or **BigQuery** (serverless) |
| "Minimize cost" + training | -> **Preemptible/Spot VMs** + right-size machine |
| "Minimize cost" + serving | -> **Batch prediction** or **scale-to-zero** |
| "Minimize latency" + serving | -> **Online prediction** + **GPU** + **Feature Store online** |
| "Maximize model performance" | -> **Custom Training** (full control, custom architecture) |
| "Team has no ML expertise" | -> **AutoML** or **Pre-built APIs** |
| "Team knows SQL" | -> **BigQuery ML** (ALWAYS!) |
| "Existing Spark code" | -> **Dataproc** (managed Spark) |
| "Prevent data exfiltration" | -> **VPC Service Controls** (NOT just IAM) |

### The Golden Rule
> When Google says "minimize operational overhead" they mean **pick the most managed/serverless option**. Eliminate any answer that requires managing clusters, VMs, or infrastructure.

---

## CHEAT SHEET 5: Vertex AI Complete Service Map

| Service | What it does | Exam keyword |
|---|---|---|
| **Custom Training** | Run training with your own code | "custom model", "PyTorch/TF code", "GPU/TPU" |
| **AutoML** | Automated model training | "no ML expertise", "minimize effort" |
| **Prediction (Endpoints)** | Host models for online serving | "deploy model", "real-time", "traffic splitting" |
| **Pipelines** | Serverless ML pipeline orchestration | "automate training", "end-to-end pipeline" |
| **Feature Store** | Centralized feature repository | "feature reuse", "training-serving consistency" |
| **Model Monitoring** | Detect drift, skew, attribution changes | "data drift", "concept drift", "monitor production" |
| **Experiments** | Track and compare training runs | "compare models", "track experiments" |
| **Model Registry** | Version and manage models | "model versioning", "model governance" |
| **Workbench** | Managed JupyterLab notebooks | "notebook", "prototyping" |
| **Data Labeling** | Human labeling service | "label data", "annotation" |
| **Vizier (HP Tuning)** | Bayesian hyperparameter optimization | "hyperparameter tuning", "find best learning rate" |
| **Matching Engine** | Vector search / ANN | "similarity search", "embedding lookup" |
| **Studio** | UI for prompt design/testing Gen AI | "prompt engineering", "test Gemini" |
| **Model Garden** | Catalog of foundation models | "browse models", "deploy pre-trained model" |
| **Batch Prediction** | Async predictions on large datasets | "bulk scoring", "nightly predictions" |
| **ML Metadata** | Track artifacts, lineage, provenance | "lineage", "artifact tracking" |

---

## CHEAT SHEET 6: Gen AI / Gemini Topics (NEW in 2026)

### Prompt Engineering vs Fine-Tuning vs RAG Decision Tree

```
Does the base model already do this well with good prompts?
  YES -> Prompt Engineering (cheapest, fastest)
  NO  -> Do you need the model to use specific/current enterprise data?
           YES -> RAG (retrieval-augmented generation)
           NO  -> Do you need different style/behavior/domain expertise?
                    YES -> Fine-Tuning (supervised or RLHF/adapter)
                    NO  -> Custom Model Training
```

### Safety & Responsible Gen AI

| Tool | Purpose | Exam keyword |
|---|---|---|
| **Model Armor** | Block malicious prompts/responses | "prompt injection", "safety filter" |
| **Safety filters** | Built-in content filtering | "inappropriate content", "harmful output" |
| **Grounding** | Anchor responses in factual data | "hallucination", "factual accuracy" |
| **Responsible AI Principles** | Ethical AI framework | "bias", "fairness", "transparency" |

### LLM Evaluation Metrics

| Metric | Measures | Use when |
|---|---|---|
| **BLEU** | N-gram precision vs reference | Translation quality |
| **ROUGE** | N-gram recall vs reference | Summarization quality |
| **Human evaluation** | Human judges rate quality | Gold standard (expensive) |
| **LLM-as-judge** | Another LLM evaluates output | Scalable automated evaluation |
| **Groundedness** | Output supported by source docs | RAG evaluation |

### Gen AI Cost Optimization

| Technique | How it helps |
|---|---|
| **Context caching** | Cache repeated system prompts, pay once |
| **Shorter prompts** | Fewer input tokens = lower cost |
| **Smaller model** | Gemini Flash for simple tasks instead of Pro/Ultra |
| **Batch API** | Lower per-token cost for non-real-time |
| **Distillation** | Train smaller model from larger one's outputs |

---

# PART 5: DOMAIN 1 - ARCHITECTING LOW-CODE AI SOLUTIONS (13%)

---

### Q1
**Your marketing team has millions of rows of customer purchase data in BigQuery. They want to predict customer churn. The team knows SQL but has no Python or ML experience. What should you recommend?**

A. Export data to Cloud Storage and train a custom TensorFlow model on Vertex AI
B. Use BigQuery ML to create a logistic regression or XGBoost model
C. Use Vertex AI AutoML Tables
D. Use the Natural Language API to classify customers

**Correct Answer: B**

**Simple Explanation:** Data is already in BigQuery, team knows SQL. BigQuery ML lets them build ML models using SQL queries directly -- no data movement, no Python needed. `CREATE MODEL` with logistic regression or XGBoost handles binary classification perfectly.

**Why others are wrong:**
- **A:** Requires Python expertise the team doesn't have, plus unnecessary data export.
- **C:** AutoML would work but requires data export and a different interface -- unnecessary when BQML does it in-place with SQL.
- **D:** Natural Language API is for text analysis, not tabular churn prediction.

---

### Q2
**A retail company wants to categorize product images into predefined categories. Their data science team is small and they want to minimize custom code. Which approach?**

A. Train a custom CNN using Vertex AI Custom Training
B. Use the Cloud Vision API's label detection feature
C. Use Vertex AI AutoML Image Classification
D. Use BigQuery ML with a DNN model

**Correct Answer: C**

**Simple Explanation:** AutoML Image Classification is purpose-built: upload labeled images, it trains a classifier using your specific categories. Minimal code.

**Why others are wrong:**
- **A:** Custom CNN requires significant ML expertise and code.
- **B:** Vision API uses Google's predefined labels, not your custom categories.
- **D:** BigQuery ML handles tabular data, not images.

---

### Q3
**A healthcare company needs to extract patient names, dates, and medication names from scanned medical forms (PDFs). They want minimal training. What service?**

A. Cloud Vision API OCR + custom regex parsing
B. Document AI with a specialized medical parser
C. Vertex AI AutoML Text Entity Extraction
D. Natural Language API entity analysis

**Correct Answer: B**

**Simple Explanation:** Document AI has specialized parsers for medical/healthcare documents that extract named fields from forms. Handles OCR + field extraction in one service.

**Why others are wrong:**
- **A:** Vision API OCR extracts raw text but doesn't understand document structure. Regex is fragile.
- **C:** AutoML requires labeled training data -- not "minimal training."
- **D:** Natural Language API does general entity recognition on plain text, not structured form extraction.

---

### Q4
**Team wants time-series forecasting for daily sales (3 years history in BigQuery). Quick turnaround, minimal infrastructure. Best approach?**

A. Export to CSV and use Prophet in a Vertex AI Notebook
B. Use BigQuery ML with the ARIMA_PLUS model type
C. Train a custom LSTM on Vertex AI with GPUs
D. Use Vertex AI AutoML Forecasting

**Correct Answer: B**

**Simple Explanation:** BigQuery ML's ARIMA_PLUS handles seasonality, holidays, trend detection automatically. Data stays in BigQuery, just one SQL query.

**Why others are wrong:**
- **A:** Prophet requires data export, Python coding, notebook management.
- **C:** Custom LSTM is overkill for standard forecasting.
- **D:** AutoML Forecasting requires data export and longer training. BQML is faster for data already in BigQuery.

---

### Q5
**E-commerce company needs to translate product descriptions to 15 languages in real-time. 10,000 products daily. Most cost-effective approach?**

A. Fine-tune a custom AutoML Translation model for each language pair
B. Use the Cloud Translation API
C. Use Gemini to translate text via Vertex AI
D. Train a seq2seq model on Vertex AI Custom Training

**Correct Answer: B**

**Simple Explanation:** Cloud Translation API is pre-built, pay-per-character, supports 100+ languages, scales automatically. No training needed.

**Why others are wrong:**
- **A:** 15 separate AutoML models is expensive overkill.
- **C:** Gemini is far more expensive per token for straightforward translation.
- **D:** Custom seq2seq for 15 language pairs is massive engineering with no benefit.

---

### Q6
**Company wants a chatbot using a foundation model that answers questions about their products using their documentation. What approach?**

A. Fine-tune a Gemini model on all product documentation
B. Use RAG with Gemini and a vector database
C. Train a custom transformer from scratch
D. Use the Natural Language API for question answering

**Correct Answer: B**

**Simple Explanation:** RAG retrieves relevant chunks at query time and feeds them as context to Gemini. Keeps answers grounded, avoids hallucination, knowledge base can be updated without retraining.

**Why others are wrong:**
- **A:** Fine-tuning teaches style/format, not factual recall. Can still hallucinate. Expensive to update.
- **C:** Training from scratch requires enormous data and compute.
- **D:** Natural Language API does entity/sentiment analysis, not Q&A over custom documents.

---

### Q7
**Data analyst needs to explore natural groupings in a customer dataset (50 features, BigQuery). No labeled data. Fastest approach?**

A. Use BigQuery ML with K-means clustering
B. Use Vertex AI AutoML Tables for classification
C. Export to notebook and run DBSCAN with scikit-learn
D. Use the Recommendations AI service

**Correct Answer: A**

**Simple Explanation:** K-means in BigQuery ML: unsupervised (no labels needed), runs via SQL, one query: `CREATE MODEL ... OPTIONS(model_type='kmeans', num_clusters=5)`.

**Why others are wrong:**
- **B:** AutoML Tables requires labeled data. They have none.
- **C:** DBSCAN requires data export, Python, doesn't scale as easily.
- **D:** Recommendations AI is for product recommendations, not clustering.

---

### Q8
**Select a foundation model from Model Garden for text summarization. Need low latency (<500ms), moderate quality, cost-efficiency for high volume. Best approach?**

A. Always select the largest available model
B. Select the smallest model that meets quality requirements, optimize with prompt engineering
C. Fine-tune the largest model on multiple GPUs
D. Use a custom-trained T5 model

**Correct Answer: B**

**Simple Explanation:** For cost + low latency, start with a smaller model (Gemini Flash vs Pro/Ultra). Prompt engineering bridges quality gaps without increasing cost.

**Why others are wrong:**
- **A:** Largest = highest latency + cost. Violates requirements.
- **C:** Fine-tuning the largest makes cost/latency worse.
- **D:** Custom T5 requires training, hosting, maintenance.

---

### Q9
**GPS tracking data arriving in real-time streams. Predict delivery times using streaming + historical data in BigQuery. Best architecture?**

A. Use Dataflow to process streams, write features to Feature Store, serve predictions via Vertex AI endpoint
B. Use BigQuery ML with real-time streaming insert and ARIMA model
C. Use Cloud Functions to process each GPS ping and call Directions API
D. Batch-process GPS data nightly in BigQuery

**Correct Answer: A**

**Simple Explanation:** Needs real-time feature computation + predictive model. Dataflow handles stream processing, Feature Store provides consistent low-latency serving, custom model gives real-time predictions.

**Why others are wrong:**
- **B:** BigQuery predictions have higher latency than an online endpoint.
- **C:** Directions API gives routing ETAs but doesn't learn from historical patterns.
- **D:** Nightly batch defeats real-time GPS purpose.

---

### Q10
**AutoML image classification model performs well but latency too high for mobile app (needs <50ms). What to do?**

A. Increase replicas on endpoint
B. Export model and use AutoML Edge for optimized edge model
C. Retrain with more data to improve latency
D. Switch to Cloud Vision API

**Correct Answer: B**

**Simple Explanation:** AutoML Edge exports models optimized for on-device inference (TF Lite, Core ML). Runs on mobile device, eliminates network roundtrip.

**Why others are wrong:**
- **A:** More replicas reduce queue wait but not network roundtrip.
- **C:** More data improves accuracy, not latency.
- **D:** Vision API has predefined labels and is cloud-based (same latency problem).

---

### Q11
**BigQuery ML model for demand forecasting. Need predictions every Monday automatically. Simplest approach?**

A. Vertex AI Pipeline
B. Scheduled query in BigQuery calling ML.PREDICT
C. Cloud Function triggered by Cloud Scheduler
D. Airflow DAG on Cloud Composer

**Correct Answer: B**

**Simple Explanation:** BigQuery has built-in scheduled queries. Schedule your `ML.PREDICT` query to run every Monday. No extra infrastructure.

**Why others are wrong:**
- **A, C, D:** All add unnecessary services when BigQuery has built-in scheduling.

---

### Q12
**Startup wants sentiment analysis for 1,000 reviews/day. No ML team. Fastest, most cost-effective solution?**

A. Train AutoML Text Sentiment model
B. Use Natural Language API's sentiment analysis
C. Fine-tune BERT on Vertex AI
D. BigQuery ML text classification

**Correct Answer: B**

**Simple Explanation:** Natural Language API has pre-built sentiment analysis, works out of the box. No training, no labeled data, no ML team needed.

**Why others are wrong:**
- **A:** Requires labeled training data and training time.
- **C:** Requires ML expertise, labeled data, GPU training.
- **D:** Requires labeled data, less accurate for sentiment than purpose-built API.

---

### Q13
**Evaluating BigQuery ML vs AutoML Tables. Dataset: 500M rows in BigQuery. Accuracy is top priority, team can wait. Which and why?**

A. BigQuery ML -- handles large datasets natively
B. AutoML Tables -- performs neural architecture search for higher accuracy
C. Both give identical accuracy
D. Neither -- use Custom Training with XGBoost

**Correct Answer: B**

**Simple Explanation:** When accuracy is top priority, AutoML Tables does automated architecture search and advanced feature engineering, typically outperforming single BQML models on complex data.

**Why others are wrong:**
- **A:** BQML is convenient but limited architectures per query.
- **C:** They do NOT give identical accuracy. AutoML generally achieves higher through search.
- **D:** Manual tuning could match but requires significant expertise.

---

### Q14
**Video streaming company wants to detect/tag objects, scenes, activities in uploaded video. 500 hours/day. Which service?**

A. Cloud Vision API on extracted frames
B. Video Intelligence API
C. AutoML Video Classification
D. Custom 3D CNN on Vertex AI

**Correct Answer: B**

**Simple Explanation:** Video Intelligence API is purpose-built for video analysis: objects, labels, activities, explicit content. Handles temporal information natively. No training needed.

**Why others are wrong:**
- **A:** Frame-by-frame loses temporal/motion context.
- **C:** Requires labeled data for custom categories.
- **D:** Massive engineering for standard tagging.

---

### Q15
**Optimize cost of running Gemini for customer service (50K queries/day). Which TWO strategies?**

A. Use prompt caching for repeated system instructions
B. Always use largest Gemini model
C. Use Gemini Flash instead of Pro for straightforward queries
D. Increase max output token limit

**Correct Answers: A and C**

**Simple Explanation:**
- **A:** Prompt caching caches static parts, pay full price once.
- **C:** Gemini Flash is much cheaper per token for routine queries.

**Why others are wrong:**
- **B:** Largest model = opposite of cost optimization.
- **D:** More output tokens = more cost.

---

# PART 6: DOMAIN 2 - COLLABORATING TO MANAGE DATA AND MODELS (16%)

---

### Q16
**Feature has different distribution at serving time vs training time. Predictions degrading. What problem and best solution?**

A. Concept drift -- retrain on recent data
B. Training-serving skew -- use Feature Store for consistent feature computation
C. Data drift -- add more training data
D. Label leakage -- remove the feature

**Correct Answer: B**

**Simple Explanation:** Same feature computed differently during training vs serving = training-serving skew. Feature Store is the single source of truth for both.

**Why others are wrong:**
- **A:** Concept drift is when feature->target relationship changes, not computation inconsistency.
- **C:** Data drift is when distributions change naturally over time.
- **D:** Label leakage is when target info leaks into features.

---

### Q17
**5 data scientists need shared notebooks with GPU access within a VPC. Which environment?**

A. Local Jupyter with shared GCS
B. Vertex AI Workbench Instances with VPC peering
C. Google Colab free tier
D. AI Platform Notebooks (legacy)

**Correct Answer: B**

**Simple Explanation:** Workbench: managed notebooks, GPU access, VPC integration, collaboration. Current Google Cloud product for enterprise notebook environments.

**Why others are wrong:**
- **A:** No centralized GPU access or VPC security.
- **C:** No VPC restrictions, limited GPU, not enterprise-grade.
- **D:** Deprecated/legacy product.

---

### Q18
**Explore new dataset with 200+ columns in BigQuery (10TB). Most efficient data quality check?**

A. Export to CSV, use pandas
B. Use TFDV to auto-generate statistics and detect anomalies
C. Write SQL for each column individually
D. Use Dataprep for visual profiling

**Correct Answer: B**

**Simple Explanation:** TFDV automatically generates statistics for ALL columns: distributions, missing values, anomalies, type issues. Scales via Dataflow.

**Why others are wrong:**
- **A:** Can't export/handle 10TB in pandas.
- **C:** SQL for 200+ columns is extremely time-consuming.
- **D:** Dataprep works but doesn't integrate as well into ML pipeline (schema for TFX).

---

### Q19
**Model uses "user_city" feature (500 unique cities in training). At serving, unknown city appears. Best handling?**

A. Return error
B. Use feature hashing
C. Manual lookup table
D. Drop city feature

**Correct Answer: B**

**Simple Explanation:** Feature hashing maps any value (including unseen) to a fixed-size vector. No vocabulary management, no errors.

**Why others are wrong:**
- **A:** Terrible user experience.
- **C:** Doesn't scale, constant maintenance.
- **D:** Loses useful predictive feature.

---

### Q20
**Compare 5 model architectures. Track metrics, hyperparameters, artifacts. What tools?**

A. Google Sheet
B. Vertex AI Experiments with SDK
C. MLflow on self-managed GKE
D. Custom BigQuery logging

**Correct Answer: B**

**Simple Explanation:** Vertex AI Experiments: managed experiment tracking, comparison dashboards, native integration. The SDK makes logging easy.

**Why others are wrong:**
- **A:** No artifact tracking, doesn't version, doesn't scale.
- **C:** Adds infrastructure management overhead.
- **D:** Reinventing what Experiments provides.

---

### Q21
**PII in training data (names, emails, phones in free text). Best approach to protect?**

A. Manual review
B. Cloud DLP API to detect and de-identify PII
C. Encrypt with CMEK
D. IAM to restrict access

**Correct Answer: B**

**Simple Explanation:** DLP API automatically detects PII and de-identifies via redaction, masking, or tokenization. Scales to large datasets.

**Why others are wrong:**
- **A:** Doesn't scale, humans miss things.
- **C:** Encryption doesn't remove PII from training. Model still learns patterns.
- **D:** Controls who accesses data but doesn't remove PII from it.

---

### Q22
**"Average purchase amount" computed differently in training (batch SQL) vs serving (application code with hardcoded stats from 3 months ago). Root cause and fix?**

A. Overfitting -- regularization
B. Training-serving skew -- standardize using Feature Store or tf.Transform
C. Need more data
D. Serving infrastructure undersized

**Correct Answer: B**

**Simple Explanation:** Different logic in training (SQL) vs serving (application code) = training-serving skew. Even small differences cause prediction issues. Use one preprocessing path.

**Why others are wrong:**
- **A:** Overfitting shows gap between training and validation during training.
- **C:** More data doesn't fix inconsistent computation.
- **D:** Infrastructure sizing affects latency, not accuracy.

---

### Q23
**Track model lineage: dataset version, preprocessing, training run, endpoint. What tool?**

A. Vertex AI ML Metadata
B. Cloud Audit Logs
C. Model Registry only
D. Git for model files

**Correct Answer: A**

**Simple Explanation:** ML Metadata tracks the full lineage chain: datasets -> preprocessing -> training -> artifacts -> endpoints.

**Why others are wrong:**
- **B:** Audit logs track API calls, not ML lineage.
- **C:** Model Registry tracks versions but not upstream lineage.
- **D:** Git tracks code, not data versions or artifacts.

---

### Q24
**Model accuracy declining over 6 months. No code changes. Input feature distributions appear stable. What drift?**

A. Data drift
B. Training-serving skew
C. Concept drift
D. Feature attribution drift

**Correct Answer: C**

**Simple Explanation:** Stable inputs + declining accuracy = the relationship between features and target has changed. This is concept drift.

**Why others are wrong:**
- **A:** Data drift means input distributions change -- question says they're stable.
- **B:** Training-serving skew is a pipeline inconsistency, not gradual decline.
- **D:** Feature attribution drift is a symptom; concept drift is the root cause.

---

### Q25
**Preprocess 2 million images (resize, normalize, augment) before training. Best approach?**

A. Local Python script with PIL
B. Dataflow with Apache Beam
C. tf.data API with preprocessing layers inside training pipeline
D. Manually preprocess and re-upload

**Correct Answer: C**

**Simple Explanation:** tf.data handles preprocessing on-the-fly during training. Augmentation varies each epoch. CPU preprocesses while GPU trains. No separate step needed.

**Why others are wrong:**
- **A:** Doesn't parallelize well, creates storage duplication.
- **B:** Overkill for standard augmentation. Augmentation should vary per epoch.
- **D:** Doesn't scale, augmentation should vary.

---

### Q26
**Real-time fraud detection needs features like "transactions in last 5 minutes." How to architect?**

A. Precompute nightly in BigQuery, cache in Redis
B. Dataflow streaming to compute real-time aggregations, write to Feature Store for online serving
C. Compute in application code at prediction time
D. BigQuery streaming inserts with scheduled ML.PREDICT

**Correct Answer: B**

**Simple Explanation:** Fraud detection needs real-time features. Dataflow streaming computes windowed aggregations, Feature Store provides low-latency lookups.

**Why others are wrong:**
- **A:** Nightly batch can't provide "last 5 minutes" features.
- **C:** Complex windowed aggregations in app code is error-prone, creates skew.
- **D:** BigQuery adds latency, scheduled queries can't provide real-time recency.

---

### Q27
**15% of "user_age" values are missing. How to handle for production ML?**

A. Drop all rows with missing values
B. Fill with mean/median and add "is_age_missing" indicator feature
C. Fill with 0
D. Fill with -1 as sentinel

**Correct Answer: B**

**Simple Explanation:** Imputing with mean/median preserves distribution. Binary indicator lets model learn if missingness is predictive. Dropping 15% wastes training signal.

**Why others are wrong:**
- **A:** Loses significant data, may introduce bias.
- **C:** 0 is not a valid age, skews distribution.
- **D:** -1 treated as actual numeric value, distorts model.

---

### Q28
**Feature Store has "customer_lifetime_value" updated daily. Request comes at 2 PM, last update at midnight. Problem?**

A. Yes -- switch to real-time computation
B. No -- CLV is slowly-changing, 14-hour staleness is acceptable
C. Yes -- stop serving until refreshed
D. No -- Feature Store always serves real-time

**Correct Answer: B**

**Simple Explanation:** CLV changes slowly (aggregate over history). 14-hour-old value is nearly identical to current. Feature freshness depends on how quickly the feature changes.

**Why others are wrong:**
- **A:** Real-time for slowly-changing features is expensive and unnecessary.
- **C:** Halting for acceptable staleness causes unnecessary downtime.
- **D:** Feature Store serves most recently ingested value, not real-time.

---

### Q29
**Model uses features from BigQuery (batch) AND Pub/Sub (streaming). How to ensure consistency?**

A. BigQuery for training, application code for serving
B. Feature Store for both, with Dataflow writing streaming and BigQuery writing batch
C. Train on batch only, ignore streaming
D. Log serving features, retrain on logs only

**Correct Answer: B**

**Simple Explanation:** Feature Store ingests from multiple sources. During training, read from Feature Store (point-in-time correct). During serving, read latest values. Same store = consistency.

**Why others are wrong:**
- **A:** Different code paths = training-serving skew.
- **C:** Ignoring streaming features degrades quality.
- **D:** Doesn't solve consistency, introduces feedback loop.

---

### Q30
**Comparing two experiments: Run A has 92% accuracy but 200ms inference. Run B has 88% accuracy but 10ms inference. Product requires sub-50ms latency. Which to promote?**

A. Run A -- higher accuracy always wins
B. Run B -- meets latency requirement
C. Run A and optimize latency later
D. Neither -- find one with both

**Correct Answer: B**

**Simple Explanation:** Run A's 200ms violates the hard sub-50ms constraint. Run B meets the requirement. Can't ship a model that doesn't meet latency SLAs.

**Why others are wrong:**
- **A:** Accuracy doesn't matter if latency requirement is violated.
- **C:** "Optimize later" is risky -- may not achieve 4x speedup.
- **D:** Run B already meets requirements. Optimize in next iteration.

---

# PART 7: DOMAIN 3 - SCALING PROTOTYPES INTO ML MODELS (21% - LARGEST)

---

### Q31
**Retail company: forecast weekly sales for 500 stores. Data in BigQuery, seasonal patterns, SQL analysts (no Python). Minimize dev time.**

A. Custom LSTM on Vertex AI
B. BigQuery ML ARIMA_PLUS
C. AutoML Forecasting
D. Prophet on Dataproc

**Correct Answer: B**

**Simple Explanation:** ARIMA_PLUS in BQML: time-series forecasting directly on BigQuery data via SQL. Handles seasonality automatically. Fastest path.

**Why others are wrong:**
- **A:** LSTM requires Python expertise, overkill.
- **C:** AutoML adds unnecessary complexity when BQML works.
- **D:** Requires Python/PySpark skills, cluster management.

---

### Q32
**Data scientist has working XGBoost model in notebook with custom feature engineering. Need to scale to 500GB with HP tuning. Keep existing Python code.**

A. Rewrite to BigQuery ML XGBoost
B. AutoML Tabular
C. Package in custom container, use Custom Training + Vizier
D. Bigger Workbench instance

**Correct Answer: C**

**Simple Explanation:** Custom Training keeps existing code as-is (containerized). Vizier handles HP tuning. "Scale up without rewriting."

**Why others are wrong:**
- **A:** Rewriting loses custom feature engineering (hard in SQL).
- **B:** AutoML doesn't support custom feature engineering logic.
- **D:** Single notebook doesn't scale to 500GB or provide HP tuning.

---

### Q33
**PyTorch model with standard dependencies needs to run on Vertex AI. No special system libraries.**

A. Build custom Docker from scratch
B. Use pre-built PyTorch container, provide code as Python package
C. Convert to TensorFlow
D. Use AutoML

**Correct Answer: B**

**Simple Explanation:** Pre-built containers already have PyTorch + torchvision. Just package your Python code. No Docker expertise needed.

**Why others are wrong:**
- **A:** Unnecessary when pre-built container exists.
- **C:** Never convert frameworks unnecessarily.
- **D:** AutoML doesn't support custom architectures.

---

### Q34
**Tune 8 hyperparameters with 50 trial budget. Find best combination efficiently.**

A. Grid search
B. Random search
C. Vertex AI Vizier with Bayesian optimization
D. Manual one-at-a-time tuning

**Correct Answer: C**

**Simple Explanation:** Bayesian optimization learns from previous trials to decide what to try next. With 8 params and 50 trials, you can't afford to waste trials.

**Why others are wrong:**
- **A:** Grid search needs thousands of trials (exponential) for 8 params.
- **B:** Random is "blind" -- doesn't learn from past trials.
- **D:** Ignores interactions between hyperparameters.

---

### Q35
**TensorFlow model fits in one GPU but 2TB dataset takes 5 days. Need under 1 day. What strategy?**

A. MirroredStrategy on 8-GPU machine
B. ParameterServerStrategy across 20 machines
C. Model parallelism
D. TPUStrategy

**Correct Answer: A**

**Simple Explanation:** Model fits in one GPU (no model parallelism needed). MirroredStrategy puts same model on all 8 GPUs, each processing different batches. ~8x speedup, simplest option.

**Why others are wrong:**
- **B:** Multi-machine is overkill when single 8-GPU machine solves it.
- **C:** Model parallelism is for models too large for one GPU.
- **D:** TPU works but more expensive and requires code changes.

---

### Q36
**Train on 10M medical images with ResNet-152. Must complete in 2 hours. Cost secondary.**

A. CPU cluster with Dataproc
B. Single machine with 4x T4 GPUs
C. TPU v3 pod slice
D. Single A100 GPU

**Correct Answer: C**

**Simple Explanation:** 10M images + ResNet-152 + 2 hours = massive parallelism needed. TPU pods have high-bandwidth interconnects, process enormous batches. Speed matters most here.

**Why others are wrong:**
- **A:** CPUs far too slow for CNNs. Would take weeks.
- **B:** 4x T4 are mid-range, insufficient for this scale and time.
- **D:** Single A100 likely can't finish in 2 hours alone.

---

### Q37
**50 billion parameter transformer. Single GPU has 40GB. Model needs 200GB. How to train?**

A. Data parallelism with MirroredStrategy across 8 GPUs
B. Model parallelism to shard model across multiple GPUs
C. Reduce model size
D. Gradient accumulation

**Correct Answer: B**

**Simple Explanation:** Model is 200GB but each GPU only has 40GB. Model literally can't fit on one GPU. Model parallelism splits the model across devices.

**Why others are wrong:**
- **A:** MirroredStrategy copies ENTIRE model to each GPU. If it doesn't fit on one, it doesn't fit on any.
- **C:** Reducing a 50B parameter model defeats the purpose.
- **D:** Gradient accumulation helps with batch size memory, not model parameter memory.

---

### Q38
**Build customer support chatbot. Have 10,000 good conversation examples. Best accuracy with reasonable cost.**

A. Train transformer from scratch
B. Gemini API with few-shot prompting (5-10 examples)
C. Fine-tune foundation model from Model Garden using 10,000 examples
D. Dialogflow CX without customization

**Correct Answer: C**

**Simple Explanation:** 10,000 examples = sweet spot for fine-tuning. Too many for prompt engineering, too few for scratch training.

**Why others are wrong:**
- **A:** 10K examples is far too few to train an LLM from scratch.
- **B:** Few-shot ignores 9,990 of your examples.
- **D:** Dialogflow without customization won't know your products.

---

### Q39
**Training job fails with OOM error. ResNet-50 on T4 GPU (16GB). Batch size 256. What to do first?**

A. Switch to A100 (80GB)
B. Reduce batch size from 256 to 32
C. Switch to CPU training
D. Rewrite model with fewer layers

**Correct Answer: B**

**Simple Explanation:** OOM = batch size too large. Each batch must fit in GPU memory. Reducing batch size is cheapest, simplest fix. Try this before bigger hardware.

**Why others are wrong:**
- **A:** Expensive overkill. ResNet-50 should train on T4 with right batch size.
- **C:** CPU training is extremely slow, doesn't solve the issue.
- **D:** ResNet-50 is a proven architecture, don't rewrite it.

---

### Q40
**Training AND validation loss both plateau at 72% accuracy (need 85%). Most likely issue?**

A. Overfitting -- add dropout
B. Underfitting -- increase model capacity
C. Learning rate too high
D. Training data has duplicates

**Correct Answer: B**

**Simple Explanation:** BOTH losses plateau equally = underfitting. If overfitting, training loss would keep dropping while validation increases. Model needs more capacity.

**Why others are wrong:**
- **A:** Overfitting = low training loss, high validation loss (gap). Here both are stuck equally.
- **C:** Too-high learning rate causes oscillation or divergence, not smooth plateau.
- **D:** Duplicates don't cause both losses to plateau identically.

---

### Q41
**Detect anomalous network traffic. No labeled attack examples. Only normal traffic data. What model type?**

A. Supervised binary classification
B. Unsupervised anomaly detection using autoencoder
C. Multi-class classification
D. Linear regression

**Correct Answer: B**

**Simple Explanation:** No labeled attacks = can't do supervised learning. Autoencoder learns "normal," flags anything it can't reconstruct well.

**Why others are wrong:**
- **A:** Needs labeled examples of both classes. Only have normal.
- **C:** Same problem + needs labels for each attack type.
- **D:** Regression predicts values, not anomalies.

---

### Q42
**Large tabular dataset (50M rows, 200 features). Highest possible accuracy. Ample compute budget.**

A. BigQuery ML logistic regression
B. AutoML Tabular
C. Vertex AI Tabular Workflows (advanced)
D. Single XGBoost via Custom Training

**Correct Answer: C**

**Simple Explanation:** Tabular Workflows is Google's most advanced automated ML for tabular data. Goes beyond AutoML with advanced architecture search and ensembling.

**Why others are wrong:**
- **A:** Logistic regression is too simple for complex 200-feature data.
- **B:** AutoML is good but Tabular Workflows provides higher accuracy.
- **D:** Single model won't match automated ensemble.

---

### Q43
**Adapt LLM for legal document analysis. 5,000 training examples. Limited GPU budget. Minimize cost.**

A. Train from scratch
B. Full fine-tuning (all parameters)
C. Adapter tuning (LoRA/PEFT) -- only train small adapter layers
D. Prompt engineering only

**Correct Answer: C**

**Simple Explanation:** LoRA adds tiny trainable layers to frozen base model. Far less GPU memory and time (10x cheaper than full fine-tuning). Sweet spot for 5K examples + limited budget.

**Why others are wrong:**
- **A:** 5K examples isn't nearly enough to train an LLM.
- **B:** Full fine-tuning updates all parameters, exceeds budget.
- **D:** 5K examples contain domain knowledge that can't fit in a prompt.

---

### Q44
**Model: 95% accuracy in training eval, 78% in production. Same data source, similar distributions. Most likely cause?**

A. Overfitting
B. Training-serving skew
C. Concept drift
D. Hardware precision errors

**Correct Answer: B**

**Simple Explanation:** High training accuracy + significantly lower serving accuracy with similar data = features computed differently at serve time. Classic training-serving skew.

**Why others are wrong:**
- **A:** Overfitting shows on validation during training. Question says training eval shows 95%.
- **C:** Same data source, similar distributions rules out concept drift.
- **D:** Hardware precision causes tiny differences, not 17% accuracy drop.

---

# PART 8: DOMAIN 4 - SERVING AND SCALING MODELS (20%)

---

### Q45
**Generate recommendations for 5M users. Can be 24 hours old. Minimize cost.**

A. Vertex AI online prediction with auto-scaling
B. Vertex AI batch prediction job nightly
C. Cloud Run with scale-to-zero
D. Real-time streaming with Dataflow

**Correct Answer: B**

**Simple Explanation:** 24-hour staleness acceptable = batch prediction. Process all 5M users cheaply in one job, cache results.

**Why others are wrong:**
- **A:** Online = paying for always-on GPU. Unnecessary when stale results are fine.
- **C:** Still doing real-time inference per user visit. Unnecessary.
- **D:** Most expensive, completely unnecessary.

---

### Q46
**Credit applications scored in real-time. Latency <200ms. 100 applications/minute peak.**

A. Batch prediction triggered per application
B. Vertex AI online prediction endpoint
C. Nightly batch pre-scoring
D. BigQuery ML ML.PREDICT

**Correct Answer: B**

**Simple Explanation:** Real-time + <200ms + per-request = online prediction. Always ready, millisecond predictions, auto-scales.

**Why others are wrong:**
- **A:** Batch has startup overhead (minutes).
- **C:** Can't pre-score unknown applicants.
- **D:** BigQuery has seconds of latency, not sub-200ms.

---

### Q47
**Deploy CatBoost model (not TF/PyTorch/sklearn/XGBoost) with custom post-processing.**

A. Pre-built sklearn container
B. Pre-built XGBoost container
C. Custom prediction container
D. Export to ONNX, use TF serving

**Correct Answer: C**

**Simple Explanation:** Pre-built containers only support TF, PyTorch, sklearn, XGBoost. CatBoost = custom container. Handles any framework + custom inference logic.

**Why others are wrong:**
- **A, B:** Different libraries with different formats.
- **D:** ONNX conversion may lose functionality, doesn't handle custom post-processing.

---

### Q48
**Test new model v2 against v1 in production. 10% traffic to v2, 90% to v1.**

A. Separate endpoint + load balancer
B. Vertex AI endpoint traffic splitting (10/90)
C. Switch 100% immediately
D. Offline evaluation on historical data

**Correct Answer: B**

**Simple Explanation:** Vertex AI endpoints natively support traffic splitting. Built-in, no custom infrastructure.

**Why others are wrong:**
- **A:** Custom infrastructure management unnecessary.
- **C:** 100% switch is risky with no safe rollback.
- **D:** Offline doesn't replace real-world testing.

---

### Q49
**Model needs 45 pre-computed features + 5 real-time features. Computing 45 at serving adds 500ms.**

A. Compute all 50 in real-time
B. Feature Store for 45 pre-computed (online serving) + combine with 5 real-time at prediction
C. Cache all in Redis, refresh hourly
D. Pre-compute predictions for all combinations

**Correct Answer: B**

**Simple Explanation:** Feature Store online serving: millisecond lookups for pre-computed features. Combine with real-time features, send to model. Total latency ~10ms + model inference.

**Why others are wrong:**
- **A:** 500ms is unacceptable for real-time serving.
- **C:** Redis works but Feature Store adds ML-specific benefits (consistency, versioning).
- **D:** Combinations explode exponentially.

---

### Q50
**Healthcare model processes PHI. Must only be accessible from VPC. No public internet.**

A. Public endpoint with API key
B. Private endpoint with VPC peering
C. Cloud Run with IAM
D. GKE with NodePort

**Correct Answer: B**

**Simple Explanation:** Private endpoints use VPC peering. All traffic stays on private network. For PHI, this is a compliance requirement.

**Why others are wrong:**
- **A:** Public endpoint sends data over internet.
- **C:** Cloud Run is publicly accessible by default.
- **D:** NodePort isn't the managed, secure approach for PHI.

---

### Q51
**Mission-critical model. New version shows 5% better accuracy. Deploy with minimal risk.**

A. Blue-green (switch all at once)
B. Canary (start with 5% traffic, monitor, gradually increase)
C. Shadow deployment
D. Direct replacement

**Correct Answer: B**

**Simple Explanation:** Canary: send 5% traffic to new model, monitor. If issues, instantly route back. Limits blast radius.

**Why others are wrong:**
- **A:** All users affected if there's an issue.
- **C:** Shadow tests but doesn't serve users.
- **D:** Riskiest, no rollback.

---

### Q52
**Sklearn random forest (100 trees, 10 features). <100ms latency. 50 req/s. What hardware?**

A. NVIDIA A100 GPU
B. NVIDIA T4 GPU
C. CPU-only (n1-standard-2)
D. TPU v3

**Correct Answer: C**

**Simple Explanation:** Random forest is tiny. CPU inference is sub-millisecond. GPUs add cost with zero benefit -- tree models don't use GPU parallelism. Don't buy a sports car to drive to the mailbox.

**Why others are wrong:**
- **A:** A100 at ~$3/hr is insane overkill.
- **B:** T4 is unnecessary. sklearn doesn't have GPU implementations.
- **D:** TPUs can't run sklearn.

---

### Q53
**Object detection on security cameras at 100 stores. Intermittent internet. <50ms per frame.**

A. Stream all frames to cloud endpoint
B. Deploy to edge devices (Coral/Edge TPU) at each store
C. Store frames, batch during connectivity windows
D. Cloud Vision API

**Correct Answer: B**

**Simple Explanation:** Intermittent internet + 50ms latency = must process locally on edge. No network dependency, no latency from round-trips.

**Why others are wrong:**
- **A:** Requires reliable internet (don't have it) + network latency exceeds 50ms.
- **C:** No real-time detection during offline windows.
- **D:** Requires internet, adds network latency.

---

### Q54
**10 small models, 10 req/s each, 10 separate endpoints. Reduce cost.**

A. Combine all into one model
B. Deploy multiple models to single endpoint (co-hosting)
C. Move all to Cloud Functions
D. Switch to batch prediction

**Correct Answer: B**

**Simple Explanation:** Co-hosting shares resources instead of 10 machines running 10% utilized.

**Why others are wrong:**
- **A:** Different models with different inputs/outputs can't be combined.
- **C:** May not support all model types, adds cold start.
- **D:** Batch doesn't work for real-time features.

---

### Q55
**Deployed v3, accuracy dropped 15% vs v2. Need immediate fix.**

A. Retrain and deploy v4
B. Route 100% traffic back to v2 via traffic splitting
C. Delete v3, redeploy v2
D. Debug v3 in production

**Correct Answer: B**

**Simple Explanation:** v2 is still on the endpoint (0% traffic). Just shift traffic split to 100% v2. Takes effect in seconds. Fix v3 offline.

**Why others are wrong:**
- **A:** Retraining takes hours. Users suffering NOW.
- **C:** Unnecessary downtime if v2 is still deployed.
- **D:** Roll back first, debug later.

---

### Q56
**TF model endpoint p99 = 800ms (SLA: 200ms). Model inference: 150ms. Bottleneck: Python preprocessing.**

A. Faster GPU
B. Rewrite preprocessing as tf.function in SavedModel graph
C. Add more replicas
D. Reduce model size

**Correct Answer: B**

**Simple Explanation:** Bottleneck is Python preprocessing (650ms), not model. tf.function compiles to C++ graph operations, eliminating Python overhead.

**Why others are wrong:**
- **A:** GPU won't help -- bottleneck is CPU Python preprocessing.
- **C:** More replicas increase throughput, not per-request latency.
- **D:** Model already fast at 150ms.

---

### Q57
**Global users. Asia = 500ms latency, US = 50ms. Endpoint in us-central1. Need Asia <100ms.**

A. Deploy second endpoint in asia-southeast1, use global load balancing
B. Increase machine type
C. Enable CDN caching
D. Bigger batch size

**Correct Answer: A**

**Simple Explanation:** 500ms is physics -- network round-trip Asia to US. Put model closer to Asian users. Global load balancing routes to nearest endpoint.

**Why others are wrong:**
- **B:** Bigger machine doesn't reduce network latency.
- **C:** Predictions are unique per request, can't cache.
- **D:** Batch size doesn't affect network latency.

---

### Q58
**Sensitive financial data model. Need: authorized access only, encrypted in transit, audit logs, not internet-accessible.**

A. Public endpoint with API key, SSL, Cloud Logging, firewall
B. Private endpoint with VPC peering, IAM auth, request-response logging, VPC Service Controls
C. Public endpoint with OAuth, SSL, BigQuery logs, Cloud Armor
D. Private endpoint with basic auth, TLS, custom audit app, IP allowlist

**Correct Answer: B**

**Simple Explanation:** Private endpoint (no internet) + IAM (authorized only) + request-response logging (audit) + VPC-SC (prevent exfiltration) + SSL by default. Complete security package.

**Why others are wrong:**
- **A:** Public endpoint fails "not internet-accessible."
- **C:** Public endpoint fails "not internet-accessible."
- **D:** Basic auth is weak. Custom audit app is unnecessary.

---

# PART 9: DOMAIN 5 - AUTOMATING AND ORCHESTRATING ML PIPELINES (18%)

---

### Q59
**Manual process: notebooks -> pickle -> ops deploys to VM (2 weeks). Reduce to <1 day, minimal infrastructure.**

A. Kubeflow on dedicated GKE cluster
B. Vertex AI Pipelines with automated training, evaluation, deployment
C. Cloud Composer scheduling notebooks
D. Cloud Function + Cloud Scheduler + Compute Engine

**Correct Answer: B**

**Simple Explanation:** Vertex AI Pipelines is serverless, purpose-built for ML workflows. Handles training, evaluation, registry, deployment in one pipeline.

**Why others are wrong:**
- **A:** Kubeflow on GKE = managing a cluster. Violates "minimal overhead."
- **C:** Notebooks aren't designed for production pipelines -- no error handling, no artifact tracking.
- **D:** DIY solution lacks ML-specific features.

---

### Q60
**TFX pipeline running on-premises. Migrate to GCP with minimal code changes.**

A. Rewrite in Kubeflow SDK
B. Deploy TFX pipeline on Vertex AI Pipelines using TFX SDK integration
C. Convert to Cloud Functions orchestrated by Composer
D. Rewrite in BigQuery ML

**Correct Answer: B**

**Simple Explanation:** TFX has native Vertex AI Pipelines integration. Swap the orchestrator, minimal code changes.

**Why others are wrong:**
- **A:** Rewriting = maximum code changes.
- **C:** Breaking TFX into functions loses all TFX benefits.
- **D:** BigQuery ML can't replicate full TFX pipeline.

---

### Q61
**Training data sometimes has unexpected nulls that cause poor predictions. Auto-detect and block bad data.**

A. Custom Python null check
B. TFDV to generate schema from good data, ExampleValidator step
C. Cloud Monitoring alert on BigQuery table
D. BigQuery scheduled query replacing nulls with zeros

**Correct Answer: B**

**Simple Explanation:** TFDV learns "normal" schema from good data, then checks new data against it. Catches nulls, distribution shifts, type mismatches, and more.

**Why others are wrong:**
- **A:** Only catches one problem. TFDV catches many.
- **C:** Alerts notify humans after the fact, don't block pipeline.
- **D:** Replacing with zeros introduces bias silently.

---

### Q62
**Preprocessing uses Pandas normalization in training, hardcoded values in Cloud Function at serving. Problem and fix?**

A. Concept drift -- retrain monthly
B. Training-serving skew -- use tf.Transform for consistent preprocessing graph
C. Data drift -- set up Model Monitoring
D. Prediction drift -- A/B testing

**Correct Answer: B**

**Simple Explanation:** Different preprocessing code (Pandas vs Cloud Function) = textbook training-serving skew. tf.Transform creates ONE graph used identically in both.

**Why others are wrong:**
- **A:** Problem is inconsistent preprocessing, not changing world.
- **C:** Data isn't changing -- processing is different.
- **D:** A/B testing compares models, doesn't fix root cause.

---

### Q63
**MLOps Level 0 -> Level 2. What does Level 2 add that Level 1 doesn't?**

A. Automated ML pipeline (CT)
B. CI/CD for pipeline code, automated testing of data/model/pipeline before deployment
C. Feature store
D. Model monitoring

**Correct Answer: B**

**Simple Explanation:** Level 1 = automated pipeline (CT). Level 2 = adds CI/CD for the pipeline code itself. Pipeline is tested and deployed like software.

**Why others are wrong:**
- **A:** That's Level 1.
- **C, D:** Good practice but not what defines Level 1->2 jump.

---

### Q64
**Complex data pipeline: 5 sources (Cloud SQL, GCS, BigQuery, Pub/Sub, REST API), complex dependencies, daily. What orchestrator?**

A. Vertex AI Pipelines
B. Cloud Composer (managed Airflow)
C. Cloud Scheduler + Cloud Functions
D. Dataflow

**Correct Answer: B**

**Simple Explanation:** Airflow excels at complex DAGs with many data sources. Pre-built operators for all those sources. Vertex AI Pipelines is ML-focused, Airflow is general orchestration.

**Why others are wrong:**
- **A:** Optimized for ML workflows, not complex multi-source ETL.
- **C:** Can't handle complex dependencies easily.
- **D:** Dataflow processes data, doesn't orchestrate.

---

### Q65
**Pipeline should deploy model ONLY if F1 > 0.85 AND better than current model. What handles this?**

A. Custom Python component
B. TFMA Evaluator with blessing thresholds (absolute + relative)
C. Manual check after each run
D. Always deploy, use traffic splitting

**Correct Answer: B**

**Simple Explanation:** TFMA Evaluator has built-in "blessing" with absolute thresholds AND baseline comparison. Model not blessed = pipeline skips deployment.

**Why others are wrong:**
- **A:** Reinvents what TFMA already does.
- **C:** Manual defeats automation purpose.
- **D:** Deploying every model is risky.

---

### Q66
**Pipeline takes 6 hours. Only training component changes during development. Speed up iteration.**

A. Pipeline caching (unchanged steps use cached results)
B. Split into two separate pipelines
C. Use smaller dataset
D. Increase machine type

**Correct Answer: A**

**Simple Explanation:** Vertex AI Pipelines supports step-level caching. If component inputs haven't changed, reuses previous output. Preprocessing runs once, subsequent runs skip to training.

**Why others are wrong:**
- **B:** Creates operational complexity.
- **C:** Smaller dataset gives different performance metrics.
- **D:** Bigger machines cost more, don't help if bottleneck is data volume.

---

### Q67
**Set up Continuous Training: auto-retrain when new data arrives in GCS bucket.**

A. Cloud Scheduler polling every hour
B. GCS notification -> Pub/Sub -> Eventarc trigger -> Vertex AI Pipeline
C. Cron job on VM watching bucket with gsutil ls
D. Composer polling every 5 minutes

**Correct Answer: B**

**Simple Explanation:** Event-driven: system tells you when new data arrives (push) instead of constantly asking (polling). Serverless, Google-native.

**Why others are wrong:**
- **A:** Wastes resources, adds up to 1 hour latency.
- **C:** Fragile, not scalable.
- **D:** Composer is expensive for simple event trigger.

---

### Q68
**CI/CD for ML: test pipeline code, build container, push to registry, trigger pipeline. Which services?**

A. GitHub Actions -> Docker Hub -> Vertex AI Pipelines
B. Cloud Build -> Artifact Registry -> Vertex AI Pipelines
C. Jenkins on GKE -> Container Registry -> Kubeflow
D. Composer -> Artifact Registry -> Vertex AI Pipelines

**Correct Answer: B**

**Simple Explanation:** Cloud Build (native CI/CD) + Artifact Registry (recommended registry) + Vertex AI Pipelines = fully managed, Google-native MLOps stack.

**Why others are wrong:**
- **A:** Not GCP-native, more integration work.
- **C:** Managing Jenkins + GKE. Container Registry is deprecated.
- **D:** Composer is orchestrator, not CI/CD tool.

---

### Q69
**Pipeline's tf.Transform bucketizes "income" into 5 quantile-based buckets. At serving, value higher than anything in training. What happens?**

A. Request fails
B. Value placed in highest bucket (boundaries frozen from training)
C. Treated as missing
D. tf.Transform recomputes boundaries

**Correct Answer: B**

**Simple Explanation:** tf.Transform "freezes" bucket boundaries into a TF graph during training. Out-of-range values fall into the highest/lowest bucket. Graph never recomputes.

**Why others are wrong:**
- **A:** Handles out-of-range gracefully, no failure.
- **C:** Value isn't missing, just out of range.
- **D:** tf.Transform NEVER recomputes at serving. That's the whole point.

---

### Q70
**Team uses PySpark feature engineering library. Want to integrate into Vertex AI Pipeline. Terabytes of data.**

A. Rewrite in Apache Beam for Dataflow
B. Custom component that submits Dataproc Serverless batch job
C. Run PySpark inside Custom Training job
D. Convert to BigQuery SQL

**Correct Answer: B**

**Simple Explanation:** Existing PySpark -> run where it works (Dataproc Serverless, no cluster management). Wrap as pipeline component.

**Why others are wrong:**
- **A:** Massive rewrite effort, high risk.
- **C:** Custom training jobs don't have Spark installed.
- **D:** Complex PySpark logic may not convert to SQL.

---

# PART 10: DOMAIN 6 - MONITORING AI SOLUTIONS (13%)

---

### Q71
**E-commerce recommendation model deployed 6 months ago. Conversion declining. Features look similar, no code changes. What issue?**

A. Data drift
B. Training-serving skew
C. Concept drift
D. Prediction drift

**Correct Answer: C**

**Simple Explanation:** Features same (not data drift), code same (not skew), but performance declining = relationship between features and what customers buy has changed. Concept drift.

**Why others are wrong:**
- **A:** Features "look similar to training data."
- **B:** No code changes.
- **D:** Prediction drift is a symptom, not root cause.

---

### Q72
**Fraud detection model: transaction_amount mean shifted from $150 (training) to $450 (serving). What issue?**

A. Concept drift
B. Data drift
C. Training-serving skew
D. Feature attribution drift

**Correct Answer: B**

**Simple Explanation:** INPUT distribution has changed ($150 -> $450 average). Model trained on one distribution, seeing different one. Data drift.

**Why others are wrong:**
- **A:** Concept drift = input->output relationship changes, not input distributions.
- **C:** Same data processed differently, not data itself changing.
- **D:** Feature attribution drift = importance of features changes.

---

### Q73
**Training uses min-max normalization (Pandas). Serving uses z-score normalization (Go microservice). What issue and fix?**

A. Data drift -- Model Monitoring
B. Concept drift -- retrain
C. Training-serving skew -- use Feature Store or tf.Transform
D. Prediction drift -- A/B testing

**Correct Answer: C**

**Simple Explanation:** Two different normalization methods = classic training-serving skew. Use ONE preprocessing path for both.

**Why others are wrong:**
- **A:** Data isn't changing, processing is different.
- **B:** Not a changing world, it's a code bug.
- **D:** A/B testing doesn't fix root cause.

---

### Q74
**Sentiment model trained on English reviews. Company expands to Japan, Japanese reviews come in. Accuracy drops 92% -> 45%. What issue?**

A. Concept drift
B. Data drift
C. Training-serving skew
D. Model staleness

**Correct Answer: B**

**Simple Explanation:** Input data fundamentally changed (English -> Japanese). Model never saw Japanese. Extreme data drift.

**Why others are wrong:**
- **A:** Concept drift = English patterns changed. Here it's a different language entirely.
- **C:** No preprocessing inconsistency.
- **D:** Not a formal term; model wasn't trained for this data.

---

### Q75
**Detect when relationship between inputs and outputs changes over time. What monitoring?**

A. Feature distribution monitoring
B. Continuous evaluation on labeled holdout set
C. Infrastructure latency/error monitoring
D. Request volume tracking

**Correct Answer: B**

**Simple Explanation:** To detect concept drift, you need LABELED data to check if predictions are still correct. Continuous evaluation tracks accuracy/F1/AUC over time.

**Why others are wrong:**
- **A:** Feature monitoring detects DATA drift, not concept drift.
- **C:** Monitors infrastructure, not model quality.
- **D:** Business metric, not quality metric.

---

### Q76
**Explain XGBoost loan decisions to regulators. Which feature attribution method?**

A. Integrated Gradients
B. XRAI
C. Sampled Shapley
D. GradCAM

**Correct Answer: C**

**Simple Explanation:** Sampled Shapley works with ANY model (model-agnostic, black-box). XGBoost is tree-based, not differentiable = can't use gradient-based methods.

**Why others are wrong:**
- **A:** Requires differentiable model (neural networks). XGBoost is tree-based.
- **B:** XRAI is for images.
- **D:** GradCAM is for CNNs.

---

### Q77
**Explain which IMAGE REGIONS a skin condition model focused on. Which method?**

A. Sampled Shapley
B. Integrated Gradients
C. XRAI
D. LIME

**Correct Answer: C**

**Simple Explanation:** XRAI identifies which REGIONS of an image were most important. Region-based explanations for image models.

**Why others are wrong:**
- **A:** Per-feature, not per-region. Not meaningful for images.
- **B:** Pixel-level, harder to interpret than region-level.
- **D:** Not a Vertex AI native offering.

---

### Q78
**Loan model has higher false rejection for certain zip codes correlating with minorities. What TWO things to do?**

A. Remove zip code feature
B. Use Fairness Indicators to evaluate across demographic slices
C. Use What-If Tool to explore feature impacts
D. Lower prediction threshold

**Correct Answers: B and C**

**Simple Explanation:** First MEASURE bias precisely (Fairness Indicators). Then INVESTIGATE why (What-If Tool). Measure first, understand second.

**Why others are wrong:**
- **A:** Removing zip code may not fix bias -- correlated features carry same signal. "Fairness through unawareness" pitfall.
- **D:** Approves more across ALL groups without addressing disparity.

---

### Q79
**LLM chatbot for customer service. Prevent revealing internal data and prompt injection. What to implement?**

A. Fine-tune to never output sensitive data
B. Model Armor for input/output safety filters + regex PII detection
C. System prompt saying "don't reveal data"
D. Rate limiting

**Correct Answer: B**

**Simple Explanation:** Model Armor inspects both inputs (prompt injection detection) and outputs (sensitive data leaks) at infrastructure level.

**Why others are wrong:**
- **A:** Fine-tuning reduces but doesn't eliminate risk.
- **C:** System prompts easily bypassed by prompt injection.
- **D:** Rate limiting prevents volume abuse, not single crafted prompts.

---

### Q80
**Document model's intended use, limitations, ethics, fairness metrics for non-technical stakeholders. What to create?**

A. Technical README
B. Model Card
C. Pipeline DAG visualization
D. Cloud Monitoring dashboard

**Correct Answer: B**

**Simple Explanation:** Model Cards: standardized documents describing model purpose, performance, limitations, ethics -- designed for non-technical readers. "Nutrition label for ML models."

**Why others are wrong:**
- **A:** README is technical, lives in Git.
- **C:** Pipeline DAG shows build process, not characteristics.
- **D:** Infrastructure metrics, not model documentation.

---

### Q81
**Prevent training data exfiltration outside organization's boundary. Healthcare data.**

A. IAM roles
B. VPC Service Controls security perimeter
C. CMEK
D. Cloud Audit Logs

**Correct Answer: B**

**Simple Explanation:** VPC-SC creates a "fence" around resources. Even with right IAM permissions, data can't move outside the perimeter.

**Why others are wrong:**
- **A:** IAM controls WHO, not WHERE data goes.
- **C:** CMEK encrypts at rest, doesn't prevent authorized movement.
- **D:** Detects after the fact, doesn't prevent.

---

### Q82
**Feature attribution patterns changed: purchase_history contribution dropped 40% -> 10%, browsing_behavior rose 15% -> 55%. Model not retrained. What drift?**

A. Data drift
B. Concept drift
C. Feature attribution drift
D. Training-serving skew

**Correct Answer: C**

**Simple Explanation:** Relative importance of features shifted. Feature attribution drift = which features the model relies on is changing. Often indicates underlying data or concept drift.

**Why others are wrong:**
- **A:** About statistical distributions, not feature importance.
- **B:** Root cause, not the specific pattern described.
- **D:** No code/pipeline change.

---

### Q83
**Model Monitoring alerts: customer_age distribution in serving differs from training baseline. No code change. First step?**

A. Immediately retrain
B. Investigate whether change is genuine (new segment) or data quality issue
C. Disable alert
D. Roll back model

**Correct Answer: B**

**Simple Explanation:** Not all distribution shifts are problems. Investigate first: real and expected? Retrain. Data bug? Fix pipeline. Knee-jerk retraining on buggy data makes things worse.

**Why others are wrong:**
- **A:** Retraining on possibly corrupted data bakes corruption in.
- **C:** Disabling alerts defeats monitoring purpose.
- **D:** Current model may be fine if shift is expected.

---

# PART 11: CROSS-DOMAIN GOTCHA QUESTIONS

---

### Q84
**Retail company, SQL analysts, 10 years of sales data in BigQuery. Forecast for 500 categories weekly. Minimal ops overhead.**

A. BigQuery ML ARIMA_PLUS with scheduled queries
B. Custom LSTM on Vertex AI + online endpoint
C. AutoML Forecasting
D. Jupyter notebook with Prophet

**Correct Answer: A**

**Simple Explanation:** SQL team + BigQuery data + minimal ops = BigQuery ML. Always. Scheduled queries automate weekly predictions.

**Why others are wrong:**
- **B:** Requires Python, ML engineering, endpoint management.
- **C:** More operational overhead than BQML.
- **D:** Requires Python, manual data export.

---

### Q85
**Custom TF model for real-time recommendations. <50ms latency, 10K req/s. Compute-intensive embeddings.**

A. Online prediction with GPU + auto-scaling
B. Batch prediction every 5 minutes
C. Cloud Run custom container
D. Online prediction CPU-only, 100 replicas

**Correct Answer: A**

**Simple Explanation:** <50ms + 10K RPS + compute-intensive = GPU online prediction with auto-scaling. All three requirements met.

**Why others are wrong:**
- **B:** Batch = minutes latency, stale recommendations.
- **C:** Cloud Run doesn't support GPUs for this.
- **D:** CPU can't hit <50ms for compute-intensive embeddings.

---

### Q86
**Streaming clickstream + batch historical data. Same feature engineering for both. Features used for online prediction + batch retraining.**

A. Dataflow for streaming, Dataproc for batch, separate Feature Store entities
B. Dataflow (Apache Beam) for both, write to Feature Store for online and offline serving
C. Two Cloud Functions
D. BigQuery for both

**Correct Answer: B**

**Simple Explanation:** Apache Beam = SAME code for batch and streaming. Feature Store serves both online and offline. Guaranteed consistency everywhere.

**Why others are wrong:**
- **A:** Different engines = two codebases = skew risk.
- **C:** Cloud Functions not designed for heavy processing.
- **D:** BigQuery has limited streaming processing for complex windowing.

---

### Q87
**Medical images: 10,000 benign, 200 malignant. Model gets 98% accuracy. Should you be satisfied?**

A. Yes, 98% is excellent
B. No -- model could predict "benign" always for 98%. Use precision, recall, F1, AUC-PR
C. No, need 100,000 images
D. Yes, but add monitoring

**Correct Answer: B**

**Simple Explanation:** 98:2 ratio = model predicting "benign" always gets 98% accuracy. Accuracy is meaningless with class imbalance. Use precision/recall/F1/AUC-PR.

**Why others are wrong:**
- **A:** 98% accuracy is a TRAP with 98:2 imbalance.
- **C:** Dataset size isn't the issue, IMBALANCE is.
- **D:** Monitoring a bad metric over time is still bad.

---

### Q88
**Document extraction: pull fields from scanned PDF invoices. 50 sample invoices. Deploy in 2 weeks.**

A. Custom object detection on 50 images
B. Document AI with pre-trained invoice parser, fine-tune if needed
C. Vision API OCR + custom regex
D. Tesseract OCR + fine-tuned BERT

**Correct Answer: B**

**Simple Explanation:** Document AI has pre-trained invoice parsers. 50 samples enough for fine-tuning. Purpose-built tool, production-ready in days.

**Why others are wrong:**
- **A:** 50 images too few for object detection from scratch.
- **C:** Regex on OCR is brittle, different layouts break it.
- **D:** Complex pipeline, 50 samples insufficient for BERT.

---

### Q89
**Pipeline should deploy ONLY if AUC > 0.90 AND new AUC at least 0.02 higher than current model. What component?**

A. Custom Python component
B. TFMA Evaluator with blessing (absolute + relative threshold)
C. Cloud Function checking metrics
D. Vertex AI Model Monitoring

**Correct Answer: B**

**Simple Explanation:** TFMA Evaluator supports both absolute thresholds AND relative baseline comparison. Built-in "blessing" gates deployment.

**Why others are wrong:**
- **A:** Reinvents TFMA functionality.
- **C:** Adds complexity for something TFMA handles.
- **D:** Model Monitoring is for production, not pipeline gating.

---

### Q90
**Security audit requires: data stays in asia-south1, no copy to external projects, model artifacts encrypted with org keys. Which THREE features?**

A. Data residency controls, VPC Service Controls, CMEK
B. IAM deny policies, Cloud Armor, default encryption
C. VPC peering, Cloud NAT, Cloud KMS
D. Org policies, Private Google Access, Shielded VMs

**Correct Answer: A**

**Simple Explanation:**
- Data residency = keeps data in asia-south1
- VPC-SC = prevents exfiltration to external projects
- CMEK = encrypts with YOUR keys

---

### Q91
**Model on always-on endpoint, 4 GPU nodes. 100 req/hr business hours, 2 req/hr overnight. Reduce cost.**

A. Switch to batch prediction
B. Auto-scaling: min 1, max 4, scale on request rate
C. Cloud Run with GPU
D. Manual scale down each evening

**Correct Answer: B**

**Simple Explanation:** Auto-scaling: 4 nodes at peak, 1 overnight. Saves ~75% nighttime costs while maintaining availability.

**Why others are wrong:**
- **A:** Still need real-time responses for overnight requests.
- **C:** Not standard pattern for Vertex AI endpoints.
- **D:** Fragile, can't handle unexpected traffic.

---

### Q92
**Training data with timestamps (5 years). Random 80/20 split. 95% AUC on test, 72% in production. Most likely cause?**

A. Overfitting
B. Data leakage from random split on temporal data -- model "sees the future"
C. Too many missing values in production
D. Model too simple

**Correct Answer: B**

**Simple Explanation:** Random split on temporal data = training data contains future records, test data contains past records. Model learned from future data that won't be available in production. Use TIME-BASED split: train years 1-4, test year 5.

**Why others are wrong:**
- **A:** Overfitting = low test accuracy too. Test is high (95%).
- **C:** No indication of missing values.
- **D:** Too-simple model = low accuracy on both test AND production.

---

### Q93
**Startup: 100 defective + 100 non-defective product images. No ML engineers. Detect defects with 95% accuracy.**

A. Collect 10,000 more images first
B. AutoML Vision, upload 200 images, evaluate, collect more if needed
C. Vision API generic classification
D. Deploy Model Garden model without fine-tuning

**Correct Answer: B**

**Simple Explanation:** AutoML + transfer learning: even 200 images can work. Start small, evaluate, iterate. No ML engineers needed.

**Why others are wrong:**
- **A:** Try first before collecting more. AutoML might work with 200.
- **C:** Vision API doesn't know YOUR specific defects.
- **D:** Generic model won't detect your specific product defects.

---

# PART 12: TOP 10 EXAM FAILURE AREAS

1. **Training-serving skew** -- Always think: is the feature computed the SAME way in training and serving? Feature Store or tf.Transform = consistency.

2. **When to use Dataflow vs Dataproc** -- Beam/streaming/exactly-once = Dataflow. Spark/existing code = Dataproc. NEVER mix them up.

3. **TFDV vs TFMA** -- TFDV = DATA validation (schema, anomalies). TFMA = MODEL analysis (evaluation, slicing). One validates data, the other validates models.

4. **Online vs Batch prediction** -- The ONLY deciding factor is: does the user need an answer RIGHT NOW? Yes = online. No = batch (cheaper).

5. **Feature Store purpose** -- It's NOT just storage. It's CONSISTENCY (same values for training and serving) + REUSABILITY (share features across teams).

6. **Concept drift vs Data drift** -- If input distributions changed = data drift. If accuracy dropped but inputs look the same = concept drift. If code computes features differently = training-serving skew.

7. **Evaluation metrics** -- "Minimize false negatives" = optimize RECALL. "Minimize false positives" = optimize PRECISION. NEVER use accuracy alone on imbalanced data.

8. **Distributed training strategies** -- Single machine multi-GPU = MirroredStrategy. Multi-machine = MultiWorkerMirroredStrategy. Model too big for one GPU = model parallelism.

9. **MLOps maturity levels** -- Level 0 = manual everything. Level 1 = automated pipeline (CT). Level 2 = CI/CD for the pipeline code itself.

10. **Responsible AI** -- Know: Sampled Shapley (any model), Integrated Gradients (neural nets), XRAI (images). Know Model Cards, Fairness Indicators, What-If Tool. Know VPC-SC for data exfiltration prevention.

---

# EXAM DAY TIPS

1. **Read the ENTIRE question** -- Google loves long scenarios. The answer is often hidden in one phrase ("team knows SQL" = BQML, "minimize operational overhead" = serverless).

2. **Eliminate wrong answers first** -- Usually 2 answers are obviously wrong, leaving a 50/50 choice.

3. **Look for keywords:** "minimize operational overhead" = managed/serverless. "minimize cost" = spot VMs, batch, right-sizing. "maximize accuracy" = custom training.

4. **Time management** -- ~2 minutes per question. Flag difficult ones, come back.

5. **When unsure, pick the most Google-native, managed solution** -- Google wants you to use their services, not third-party tools.

6. **Remember the new branding** -- "Vertex AI" may appear as "Gemini Enterprise Agent Platform" in some questions.

---

**Total practice questions in this guide: 93**
**Cheat sheets: 6**
**You've got this. Good luck on September 21!**
