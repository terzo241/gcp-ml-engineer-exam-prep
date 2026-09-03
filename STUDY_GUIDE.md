# Google Cloud Professional Machine Learning Engineer - Exam Preparation Guide

**Exam:** PR000269 | **Date:** Monday, September 21, 2026, 4:00 PM IST | **Duration:** 135 minutes
**Location:** MINSWAY SOLUTIONS PRIVATE LIMITED

---

## EXAM OVERVIEW

| Aspect | Details |
|--------|---------|
| Questions | 50-60 multiple-choice & scenario-based |
| Duration | 120-135 minutes |
| Passing Score | ~70% (scaled scoring) |
| Cost | $200 USD |
| Validity | 2 years |
| Focus | ~60% MLOps/production ML, ~40% model building |

### June 2026 Major Update
- Transition emphasis from Vertex AI to **Gemini Enterprise Agent Platform**
- **Generative AI** heavily emphasized (Vertex AI Studio, Model Garden, RAG)
- Gemini model fine-tuning as core topic
- Agentic AI architecture added
- Certification validity reduced from 3 to 2 years

---

## EXAM DOMAINS & WEIGHTAGE

| # | Domain | Weight | Priority |
|---|--------|--------|----------|
| 1 | Architecting Low-Code AI Solutions | 13% | Medium |
| 2 | Collaborating Within & Across Teams (Data & Models) | 14% | Medium |
| 3 | Scaling Prototypes into ML Models | 17% | HIGH |
| 4 | Serving and Scaling Models | 20% | HIGHEST |
| 5 | Automating & Orchestrating ML Pipelines | 18% | HIGH |
| 6 | Monitoring AI Solutions | 10% | Medium |

**Key Insight:** Domains 3+4+5 = 55% of the exam. Master these first.

---

## 18-DAY STUDY PLAN (Sep 3 - Sep 20)

You have **18 days**. Here's an aggressive but achievable plan:

### Phase 1: Foundation (Days 1-5, Sep 3-7)
- Complete Google Cloud Skills Boost ML Learning Path
- Read official exam guide PDF end-to-end
- Watch YouTube overview videos
- **Focus:** Vertex AI components, BigQuery ML basics, GCP ML service landscape
- **Hours:** 3-4 hours/day

### Phase 2: Deep Dive (Days 6-10, Sep 8-12)
- Coursera: Production ML Systems + MLOps Fundamentals (accelerated)
- Deep study of high-weight domains (Serving, Pipelines, Scaling)
- Hands-on labs on Vertex AI, BigQuery ML, AutoML
- **Focus:** MLOps, Pipelines, Feature Store, Model Monitoring
- **Hours:** 3-4 hours/day

### Phase 3: Practice & Gaps (Days 11-15, Sep 13-17)
- Take full practice exams (Udemy 400+ questions)
- Review ExamTopics community Q&A
- Deep dive on weak areas identified from practice
- **Focus:** Scenario-based decision making, service selection
- **Target:** Score 80%+ on practice tests before moving on
- **Hours:** 3-4 hours/day

### Phase 4: Final Review (Days 16-18, Sep 18-20)
- Final full-length practice exam simulation (timed)
- Review all wrong answers and weak topics
- Quick review of Responsible AI, Generative AI topics
- Light review day before exam - don't cram
- **Hours:** 2-3 hours/day

---

## TOP STUDY RESOURCES (Priority Ranked)

### Must-Do (Free)
1. **Google Cloud Skills Boost Learning Path** - https://www.cloudskillsboost.google/paths/17
2. **Official Exam Guide PDF** - https://services.google.com/fh/files/misc/professional_machine_learning_engineer_exam_guide_english.pdf
3. **Official Certification Page** - https://cloud.google.com/learn/certification/machine-learning-engineer
4. **OpenExamPrep** - 200+ free practice questions, no signup - https://open-exam-prep.com/practice/gcp-machine-learning

### Highly Recommended (Paid)
5. **Coursera Professional Certificate** - https://www.coursera.org/professional-certificates/preparing-for-google-cloud-machine-learning-engineer-professional-certificate (free audit available)
6. **Udemy Practice Tests (400+ Qs, 2026 updated)** - ~$15 on sale
   - https://www.udemy.com/course/google-cloud-ml-engineer-practice-tests-2026-400-qs/
   - https://www.udemy.com/course/google-gcp-ml-engineer-certification-practice-updated-exam/
7. **Official Study Guide Book (Sybex/Wiley)** - by Mona Mona & Pratap Ramamurthy

### Supplementary (Free)
8. **ExamTopics Community Q&A** - https://www.examtopics.com/exams/google/professional-machine-learning-engineer/
9. **GitHub Study Guide** - https://github.com/zabir-nabil/gcp-ml-certification
10. **Towards Data Science Blog** - https://towardsdatascience.com/how-to-prepare-for-the-gcp-professional-machine-learning-engineer-exam-b1c59967355f/

### YouTube
- "How To Pass on First Attempt" - https://www.youtube.com/watch?v=1pBjGDAQj_g
- "How to Become ML Engineer" - https://www.youtube.com/watch?v=n_NTzTqRnc8

### Blogs from People Who Passed
- Josh Tan (Medium) - https://medium.com/@joshcx/how-i-passed-the-google-cloud-professional-machine-learning-engineer-exam-vertex-ai-484c7863bbac
- JPantsjoha (Google Cloud Community) - https://medium.com/google-cloud/google-cloud-machine-learning-exam-prep-broken-down-by-learning-effort-levels-21f96088a274
- Google Dev Forums (30-day pass) - https://discuss.google.dev/t/google-clouds-professional-ml-engineer-pmle-exam-how-i-passed-in-30-days-and-you-can-too/179510
- ExamCert 2026 Guide - https://www.examcert.app/blog/gcp-pmle-complete-guide/

---

## DOMAIN 1: ARCHITECTING LOW-CODE AI SOLUTIONS (13%)

### Key Topics
- Building AI solutions using ML APIs or foundation models
- Using Gemini Enterprise models for specific tasks
- Industry-specific APIs (Vision, Natural Language, Translation, Speech)
- Tuning foundation models for specific use cases
- Vertex AI Studio for generative AI prototyping

### Decision Matrix: When to Use What

| Scenario | Solution |
|----------|----------|
| No ML expertise, structured data | BigQuery ML |
| No ML expertise, images/text/video | AutoML |
| Quick prototype with foundation model | Vertex AI Studio |
| Need pre-built API (vision, NLP) | ML APIs |
| Custom architecture needed | Vertex AI Custom Training |
| Fine-tune foundation model | Gemini supervised tuning |

---

## DOMAIN 2: DATA & MODEL COLLABORATION (14%)

### Data Preprocessing Tools

| Tool | Best For | Type |
|------|----------|------|
| BigQuery | SQL-based transformations, large structured data | Serverless |
| Dataflow (Apache Beam) | Large-scale batch/streaming ETL | Serverless |
| Dataproc (Spark) | Spark/PySpark workloads | Managed cluster |
| tf.Transform | Training-serving consistency | TensorFlow native |
| Cloud Dataprep | No-code visual data prep | GUI-based |

### Feature Store (Vertex AI)
- Centralized feature management
- Online & batch serving
- Feature monitoring & governance
- Time-series feature support
- **Exam Q:** When to use Feature Store vs BigQuery = Feature Store when features shared across models/teams

### Data Preprocessing Pipeline Pattern
```
Raw Data (GCS/BigQuery)
  → Data Cleaning (Dataflow/Dataproc)
  → Feature Engineering (BigQuery/tf.Transform)
  → Feature Store (if shared)
  → Train/Validation Split
  → Model Training (Vertex Training)
```

---

## DOMAIN 3: SCALING PROTOTYPES INTO ML MODELS (17%)

### AutoML vs Custom Training vs BigQuery ML

| Criteria | BigQuery ML | AutoML | Custom Training |
|----------|-------------|--------|-----------------|
| Expertise needed | SQL only | Minimal ML | Full ML |
| Data type | Structured | Structured/Images/Text/Video | Any |
| Customization | Limited | Limited | Full control |
| Time to model | Minutes | Hours | Days-weeks |
| Best for | Quick prototypes, analysts | MVPs, limited ML team | Production, complex models |
| Model access | SQL interface | Black box | Full code access |

### BigQuery ML Model Types

| Model | Use Case |
|-------|----------|
| Linear/Logistic Regression | Prediction, classification |
| ARIMA (Time Series) | Forecasting |
| XGBoost | Tabular classification/regression |
| DNN | Complex patterns |
| K-Means | Clustering/segmentation |
| Boosted Trees | Classification with feature importance |

### BigQuery ML Key Syntax
```sql
-- Train
CREATE OR REPLACE MODEL dataset.model_name
OPTIONS(model_type='linear_reg', input_label_cols=['target'])
AS SELECT * FROM dataset.training_data;

-- Predict
SELECT * FROM ML.PREDICT(MODEL dataset.model_name,
  (SELECT * FROM dataset.new_data));

-- Evaluate
SELECT * FROM ML.EVALUATE(MODEL dataset.model_name);
```

### Hyperparameter Tuning (Vertex AI)
- **Bayesian Optimization** - most efficient (default choice)
- Grid Search - exhaustive, slow
- Random Search - faster than grid
- Use logarithmic scale for learning rate ranges
- Always evaluate on validation set

### Distributed Training
- **Data Parallelism** (most common): same model, different data batches
  - `tf.distribute.MirroredStrategy()` - single machine, multi-GPU
  - `tf.distribute.MultiWorkerMirroredStrategy()` - multi-machine
- **Model Parallelism**: model split across GPUs (for very large models)
- **Hardware:** V100, A100 GPUs; TPU v3, v4

### Transfer Learning
- Shallow fine-tuning: update top layers only (less data needed)
- Deep fine-tuning: update all layers (more data needed)
- Feature extraction: freeze all, train new head (fastest)

---

## DOMAIN 4: SERVING & SCALING MODELS (20%) - HIGHEST WEIGHT

### Deployment Patterns

| Pattern | When to Use | Latency | Cost |
|---------|-------------|---------|------|
| Online Prediction | Real-time, user-facing | <100ms | Higher |
| Batch Prediction | Bulk processing, non-urgent | N/A | Lower |
| Private Endpoints | Regulated data, no internet | <100ms | Highest |

### Model Deployment Strategies

**Canary (Traffic Splitting):**
```
Old Model → 90% traffic
New Model → 10% traffic
Monitor → Increase if metrics good, rollback if bad
```

**Blue-Green:** Two identical environments, instant switch
**Shadow/Dark Launch:** New model runs parallel without affecting users

### Scaling
- **Autoscaling:** Based on CPU/memory/request rate
- **Shared resources:** Multiple models per machine (cheaper)
- **Dedicated resources:** Guaranteed latency (expensive)
- Right-size machine types for cost optimization

### Model Registry
- Version control for models
- Deploy specific versions to endpoints
- Track model lineage and metadata
- Evaluate across model versions

---

## DOMAIN 5: ML PIPELINE AUTOMATION (18%) - HIGH WEIGHT

### Vertex AI Pipelines
- Built on Kubeflow Pipelines
- DAG-based workflow orchestration
- Integration with all Vertex AI services
- Scheduled or event-triggered execution

### Standard ML Pipeline Pattern
```
Ingest (GCS/BigQuery)
  → Preprocess (Dataflow/tf.Transform)
  → Feature Engineering (Feature Store)
  → Train (Vertex Training)
  → Evaluate (Model Evaluation)
  → Gate (quality threshold)
  → Register (Model Registry)
  → Deploy (Vertex Prediction)
  → Monitor (Model Monitoring)
```

### CI/CD for ML
```
Git Push → Cloud Build Pipeline
  ├── Unit tests
  ├── Data validation
  ├── Train on sample
  ├── Evaluate
  └── If pass → Trigger Vertex Pipeline
        → Full train → Evaluate → Register → Deploy
```

### MLOps Maturity Levels
- **Level 0:** Manual process (notebooks)
- **Level 1:** ML pipeline automation (Vertex Pipelines)
- **Level 2:** CI/CD pipeline automation (Cloud Build + Vertex)

### Key MLOps Principles
1. **Automation** - Data validation, training, evaluation, deployment
2. **Reproducibility** - Version control code, data, models, configs
3. **Monitoring** - Drift detection, quality metrics
4. **Governance** - Approval workflows, access control, audit logs

---

## DOMAIN 6: MONITORING AI SOLUTIONS (10%)

### Types of Drift

| Drift Type | What Changes | Detection |
|------------|-------------|-----------|
| Data Drift | Input feature distributions | KS test, chi-squared |
| Prediction Drift | Output distributions (no data drift) | Statistical tests |
| Label Drift | Actual target distribution | Ground truth comparison |
| Concept Drift | Relationship between features & target | Performance degradation |

### Vertex AI Model Monitoring
- Automated drift detection with thresholds
- Alerting via Cloud Logging + Pub/Sub
- Historical performance comparison
- Custom metric monitoring

### Retraining Strategies
- **Scheduled:** Weekly/daily based on time
- **Triggered:** On drift detection or quality drop
- **Incremental:** Add new data to previous training set
- **Feature-based:** Retrain only if specific features drift

### Model Evaluation Metrics

**Classification:**
| Metric | Use When |
|--------|----------|
| Accuracy | Balanced classes |
| Precision | False positives expensive (spam, fraud) |
| Recall | False negatives expensive (disease, security) |
| F1 Score | Need balance, imbalanced data |
| ROC-AUC | Evaluate across all thresholds |
| PR-AUC | Highly imbalanced data |

**Regression:**
| Metric | Use When |
|--------|----------|
| MAE | Outliers weighted equally |
| RMSE | Outliers should be penalized |
| R² | Compare against baseline |
| MAPE | Want percentage error |

**Quick Decision Framework:**
```
Balanced classes → Accuracy
Imbalanced classes → F1 or PR-AUC
FP costly → Precision
FN costly → Recall
Regression + outliers matter → RMSE
Regression + outliers don't matter → MAE
```

---

## RESPONSIBLE AI & FAIRNESS

### Bias Types to Know
- **Selection Bias:** Training data not representative
- **Measurement Bias:** Data collection errors
- **Aggregation Bias:** Ignoring subgroups
- **Evaluation Bias:** Metric doesn't capture fairness

### Fairness Metrics
- Demographic Parity, Equalized Odds, Calibration, Individual Fairness

### GCP Responsible AI Tools
- **What-If Tool:** Interactive model exploration, fairness analysis
- **Model Cards:** Document performance, limitations, ethics
- **Explainability:** Feature Attribution, SHAP, LIME, Integrated Gradients

---

## GENERATIVE AI (NEW - 2026 Focus)

### Key Topics
- **Vertex AI Studio:** Prototyping generative AI applications
- **Model Garden:** Access to foundation models
- **Gemini Fine-Tuning:** Supervised tuning, adapter tuning
  - Supported: Gemini 2.5 Pro, Flash, Flash Lite
- **RAG (Retrieval-Augmented Generation):** Architecture patterns
- **Prompt Engineering:** Best practices for production
- **Agentic AI:** Building intelligent agents on GCP

---

## EXAM-TAKING STRATEGIES

### Time Management
- ~2 minutes per question (60 Qs / 120 min)
- Flag difficult questions and move on
- Don't spend >3 min on any single question

### Answer Strategy
1. **Identify keywords:** real-time→online, batch→batch prediction, no ML expertise→AutoML
2. **Prefer managed services:** Vertex AI > open-source, BigQuery > Dataproc
3. **Eliminate wrong answers:** too expensive, too slow, too complex, not GCP-native
4. **When multiple seem correct:** choose the most fully-managed option
5. **Read carefully:** batch vs real-time, retraining vs monitoring, deploy vs serve

### Common Exam Traps
- Choosing custom training when AutoML suffices
- Using Dataproc when Dataflow is better (serverless preferred)
- Ignoring training-serving skew (tf.Transform solves this)
- Not considering cost optimization
- Overcomplicating with open-source when GCP-native works

---

## KEY SERVICE CHEAT SHEET

| Need | Service |
|------|---------|
| SQL-based ML | BigQuery ML |
| No-code ML on structured data | AutoML Tables |
| Image classification | AutoML Vision / Vision API |
| Text classification | AutoML Text / NL API |
| Custom model training | Vertex AI Training |
| Model deployment | Vertex AI Prediction |
| ML workflow orchestration | Vertex AI Pipelines |
| Feature management | Vertex AI Feature Store |
| Model versioning | Vertex AI Model Registry |
| Large-scale ETL | Dataflow (Apache Beam) |
| Spark workloads | Dataproc |
| Streaming data | Pub/Sub → Dataflow |
| Training-serving consistency | tf.Transform |
| Model monitoring | Vertex AI Model Monitoring |
| Generative AI prototyping | Vertex AI Studio |
| Foundation model access | Model Garden |
| CI/CD for ML | Cloud Build + Vertex Pipelines |

---

## PRACTICE QUESTION SAMPLES

### Q1: Service Selection
**A retail company wants analysts (no ML expertise) to predict customer churn using historical transaction data in BigQuery. Which approach is most appropriate?**

A) Train custom TensorFlow model on Vertex AI
B) Use BigQuery ML with logistic regression
C) Deploy pre-trained model from Model Garden
D) Use Dataflow to build ML pipeline

**Answer: B** - BigQuery ML is ideal for analysts (SQL-only), structured data already in BigQuery, and classification tasks.

---

### Q2: Deployment Pattern
**Your model is in production. You've trained a new version with improved accuracy. How do you safely deploy it?**

A) Replace the existing model immediately
B) Use traffic splitting: 90% old, 10% new, monitor metrics
C) Take the endpoint down, deploy new model, bring it back up
D) Run batch prediction with new model, compare results offline

**Answer: B** - Canary deployment with traffic splitting is the safest approach for production model updates.

---

### Q3: Data Drift
**Your production model's accuracy has dropped 15% over the past month, but no code changes were made. What is the most likely cause?**

A) Model overfitting during training
B) Data drift in input features
C) Incorrect hyperparameters
D) Insufficient training data

**Answer: B** - With no code changes, degradation over time is most likely due to data drift (input distribution shift).

---

### Q4: Preprocessing
**You need to ensure the same feature transformations are applied during both training and serving. Which tool should you use?**

A) Cloud Dataprep
B) BigQuery views
C) tf.Transform
D) Dataproc PySpark

**Answer: C** - tf.Transform generates both training and serving graphs, ensuring consistent preprocessing.

---

### Q5: Pipeline Automation
**Your team manually retrains models monthly. You want to automate retraining when data drift is detected. What's the best approach?**

A) Cron job to retrain every day
B) Vertex AI Model Monitoring → Pub/Sub alert → Cloud Function → Trigger Vertex Pipeline
C) Manual monitoring dashboard with email alerts
D) Dataflow streaming pipeline for continuous training

**Answer: B** - Event-driven retraining using monitoring + alerting + automated pipeline trigger is the MLOps best practice.

---

### Q6: Cost Optimization
**You need to generate predictions for 10 million records nightly for a batch reporting system. Which deployment approach minimizes cost?**

A) Online prediction endpoint with autoscaling
B) Batch prediction job
C) Private endpoint with dedicated resources
D) Multiple online endpoints with load balancing

**Answer: B** - Batch prediction is cheaper than maintaining an always-on endpoint when real-time isn't needed.

---

### Q7: AutoML vs Custom
**Your team of data scientists wants to build a custom recommendation engine with complex collaborative filtering and content-based hybrid approach. Which is most appropriate?**

A) AutoML Tables
B) BigQuery ML matrix factorization
C) Vertex AI Custom Training with TensorFlow
D) Pre-built Recommendations AI API

**Answer: C** - Complex hybrid recommendation requires custom architecture, which needs full custom training.

---

### Q8: Feature Store
**Multiple ML teams build models using the same customer features but each team computes features differently, causing inconsistency. What's the best solution?**

A) Share SQL queries between teams
B) Use Vertex AI Feature Store for centralized feature management
C) Create a shared BigQuery dataset
D) Document feature engineering steps in a wiki

**Answer: B** - Feature Store provides centralized, governed, consistent features across teams and models.

---

### Q9: Responsible AI
**Your classification model performs well overall (95% accuracy) but poorly on a minority subgroup (60% accuracy). What should you do first?**

A) Deploy the model since overall accuracy is high
B) Collect more data from the minority subgroup and retrain
C) Use the What-If Tool to analyze fairness across subgroups
D) Switch to a simpler model

**Answer: C** - First analyze the fairness issue using the What-If Tool, then determine the root cause before deciding on remediation.

---

### Q10: Distributed Training
**You're training a large image classification model and a single GPU takes 48 hours. How do you reduce training time?**

A) Use a larger GPU
B) Use tf.distribute.MirroredStrategy() for multi-GPU training
C) Reduce the dataset size
D) Lower the number of epochs

**Answer: B** - Data parallelism with MirroredStrategy distributes training across multiple GPUs for near-linear speedup.

---

### Q11: Model Monitoring
**After deploying a fraud detection model, you notice the false negative rate has increased significantly. What metric should you primarily track?**

A) Accuracy
B) Precision
C) Recall
D) F1 Score

**Answer: C** - Recall measures false negatives. For fraud detection, missing actual fraud (false negatives) is the most costly error.

---

### Q12: Generative AI (2026 NEW)
**You want to build a customer support chatbot that answers questions using your company's internal documentation. Which architecture is most appropriate?**

A) Fine-tune Gemini on all internal documents
B) Use RAG (Retrieval-Augmented Generation) with Vertex AI Search + Gemini
C) Train a custom seq2seq model from scratch
D) Use the Translation API

**Answer: B** - RAG combines retrieval of relevant documents with generative AI, ideal for knowledge-grounded chatbots without fine-tuning costs.

---

### Q13: MLOps Pipeline
**Your ML pipeline needs to: validate data quality, train a model, evaluate it, and only deploy if metrics exceed a threshold. Which is the best orchestration?**

A) Cron jobs chained with Cloud Functions
B) Vertex AI Pipeline with conditional components
C) Manual notebook execution sequence
D) Cloud Composer (Airflow) with BashOperator

**Answer: B** - Vertex AI Pipelines natively supports DAG orchestration with conditional logic and integrates with all Vertex services.

---

### Q14: Data Processing
**You need to process 5TB of raw log data for feature extraction. The data is in Cloud Storage and needs complex transformations. Which service?**

A) Cloud Dataprep
B) Dataflow with Apache Beam
C) Cloud Functions
D) Compute Engine script

**Answer: B** - Dataflow is serverless, auto-scaling, and designed for large-scale batch data processing.

---

### Q15: Transfer Learning
**You have only 500 labeled medical images for classification. Training from scratch gives poor results. What approach should you try?**

A) Collect more data (10,000+ images)
B) Use transfer learning from a pre-trained ImageNet model, fine-tune top layers
C) Use unsupervised clustering
D) Increase model complexity

**Answer: B** - Transfer learning leverages pre-trained features, requiring far less labeled data. Fine-tuning only top layers works well with small datasets.

---

### Q16: BigQuery ML
**A marketing analyst wants to segment customers into groups based on purchasing behavior using BigQuery. Which model type?**

A) Linear Regression
B) Logistic Regression
C) K-Means Clustering
D) ARIMA

**Answer: C** - K-Means clustering is the unsupervised approach for customer segmentation based on behavioral patterns.

---

### Q17: Serving Architecture
**Your model serves predictions to a mobile app with variable traffic (10 req/s to 10,000 req/s). How do you deploy cost-effectively?**

A) Fixed-size online endpoint
B) Online endpoint with autoscaling based on request rate
C) Batch prediction every hour
D) Edge deployment on each device

**Answer: B** - Autoscaling adjusts resources to match traffic, handling bursts cost-effectively.

---

### Q18: Training-Serving Skew
**Your model performs well in testing but poorly in production. Investigation shows feature values differ between training and serving. What's the root cause?**

A) Overfitting
B) Training-serving skew due to inconsistent preprocessing
C) Insufficient training data
D) Wrong model architecture

**Answer: B** - Training-serving skew occurs when preprocessing logic differs between training and serving environments. tf.Transform prevents this.

---

### Q19: Model Evaluation
**You're building a spam filter. Users complain about important emails being marked as spam. Which metric should you optimize?**

A) Recall (minimize false negatives)
B) Precision (minimize false positives)
C) Accuracy
D) F1 Score

**Answer: B** - Important emails marked as spam = false positives. Optimizing precision reduces false positives.

---

### Q20: Vertex AI Experiments
**Your team is testing 50 different hyperparameter combinations for a model. How do you efficiently track and compare results?**

A) Spreadsheet logging
B) Vertex AI Experiments with tracked metrics
C) Manual notebook comparison
D) Cloud Logging queries

**Answer: B** - Vertex AI Experiments provides structured tracking, comparison, and visualization of experiment runs.

---

### Q21: Streaming ML
**You need to make real-time fraud predictions on streaming transaction data from Pub/Sub. What architecture?**

A) Pub/Sub → BigQuery → Batch Prediction
B) Pub/Sub → Dataflow → Online Prediction Endpoint
C) Pub/Sub → Cloud Storage → Manual analysis
D) Pub/Sub → Cloud Functions → BigQuery ML

**Answer: B** - Dataflow processes streaming data from Pub/Sub and calls the online prediction endpoint for real-time inference.

---

### Q22: Vertex AI Pipelines
**Your pipeline has 5 steps. Step 3 (training) occasionally fails due to resource limits. How do you handle this?**

A) Restart the entire pipeline manually
B) Configure retry policy on the training component with exponential backoff
C) Skip step 3 if it fails
D) Run all steps in parallel

**Answer: B** - Vertex AI Pipelines support retry policies on individual components, handling transient failures automatically.

---

### Q23: Model Selection
**You need a time-series forecast for monthly sales for the next 12 months. Data is in BigQuery. What's the quickest approach?**

A) Custom LSTM model on Vertex AI
B) BigQuery ML with ARIMA_PLUS model
C) AutoML Tables regression
D) Prophet on Compute Engine

**Answer: B** - ARIMA_PLUS in BigQuery ML is purpose-built for time-series forecasting, requires only SQL, and handles seasonality automatically.

---

### Q24: Gemini Fine-Tuning (2026 NEW)
**You want to customize Gemini's responses for your domain-specific terminology and style. Your dataset has 1,000 examples. Which approach?**

A) Full pre-training from scratch
B) Supervised fine-tuning with adapter tuning on Vertex AI
C) Prompt engineering only
D) RAG with domain documents

**Answer: B** - Supervised fine-tuning with adapter tuning is parameter-efficient and works well with ~1,000 examples for domain adaptation.

---

### Q25: Data Validation
**Before training, you want to automatically detect data quality issues (missing values, schema changes, distribution shifts). What tool?**

A) BigQuery data quality rules
B) TensorFlow Data Validation (TFDV)
C) Cloud Data Loss Prevention
D) Cloud Dataprep

**Answer: B** - TFDV is purpose-built for ML data validation, detecting anomalies, schema drift, and distribution shifts in training data.

---

### Q26: Multi-Model Serving
**You have 3 models that need to run sequentially (model A output feeds model B, which feeds model C). How do you deploy this?**

A) Three separate endpoints, application orchestration
B) Single custom container with all 3 models
C) Vertex AI Pipeline for inference
D) Cloud Functions chaining

**Answer: A** - For production serving with sequential model dependencies, separate endpoints with application-level orchestration provides flexibility, independent scaling, and model versioning.

---

### Q27: Cost vs Performance
**Training costs are $5,000/run but model accuracy improvement is marginal (0.2%). Stakeholders want cheaper iterations. What do you recommend?**

A) Continue with current approach for maximum accuracy
B) Use AutoML for faster, cheaper experimentation before custom training
C) Reduce training data to lower costs
D) Switch to CPU-only training

**Answer: B** - Use AutoML for rapid cheap experimentation to identify promising approaches before investing in expensive custom training runs.

---

### Q28: Label Quality
**You have 100K images but labels are noisy (estimated 15% incorrect). What should you do before training?**

A) Train anyway - models are robust to noise
B) Use data labeling service to relabel + implement active learning for uncertain samples
C) Remove 15% of data randomly
D) Use only the first 10K images

**Answer: B** - Clean labels are critical. A data labeling service with active learning focuses human review on the most uncertain/likely-wrong labels.

---

### Q29: Edge Deployment
**You need to run an object detection model on IoT devices with limited connectivity. Which approach?**

A) Always call cloud API for prediction
B) Export model to TensorFlow Lite, deploy to edge devices
C) Use batch prediction
D) Store predictions in local database

**Answer: B** - TensorFlow Lite models run locally on edge devices, handling low-connectivity scenarios.

---

### Q30: Experiment Tracking
**Your team of 5 ML engineers runs hundreds of experiments weekly across different projects. How do you ensure reproducibility?**

A) Shared notebook with manual notes
B) Vertex AI Experiments + Vertex AI Metadata Store + containerized environments
C) Git branches per experiment
D) Email summaries of each experiment

**Answer: B** - Vertex AI Experiments tracks runs, Metadata Store captures lineage, and containers ensure environment reproducibility.

---

## LAST-MINUTE REVIEW CHECKLIST

Before walking into the exam, make sure you can answer:

- [ ] When to use BigQuery ML vs AutoML vs Custom Training?
- [ ] Online vs Batch prediction - when and why?
- [ ] What is training-serving skew and how does tf.Transform prevent it?
- [ ] How does Vertex AI Feature Store ensure feature consistency?
- [ ] What are the types of data drift and how to detect each?
- [ ] How to set up automated retraining pipelines?
- [ ] Traffic splitting for safe model deployment - how?
- [ ] Precision vs Recall - when to prioritize each?
- [ ] What is RAG and when to use it vs fine-tuning?
- [ ] Responsible AI: bias types, fairness metrics, What-If Tool
- [ ] Distributed training strategies (MirroredStrategy, MultiWorker)
- [ ] Vertex AI Pipeline components and patterns
- [ ] Gemini fine-tuning approaches (adapter vs full)
- [ ] CI/CD for ML using Cloud Build + Vertex Pipelines
- [ ] Hyperparameter tuning: Bayesian vs Grid vs Random

---

**Good luck on September 21! You've got this.**
