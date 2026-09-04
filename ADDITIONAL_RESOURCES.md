# Additional Resources & Exam Strategy

## What You MUST Also Do (non-negotiable)

1. **Google's Official Sample Questions** -- Take them first to calibrate your level
   - https://docs.google.com/forms/d/e/1FAIpQLSeYmkCANE81qSBqLW0g2X7RoskBX9yGYQu-m1TtsjMvHabGqg/viewform

2. **Hands-on Labs (Cloud Skills Boost)** -- The exam tests practical understanding, not just theory. Do at least these labs:
   - BigQuery ML (create a model, run ML.PREDICT)
   - Vertex AI Pipelines (build and run one)
   - Vertex AI Feature Store (ingest + serve features)
   - Model deployment with traffic splitting
   - https://www.skills.google/paths/17

3. **ExamTopics or Whizlabs practice tests** -- The 93 questions in STUDY_GUIDE.md cover concepts, but you need to see 200-300 more questions to build exam stamina and pattern recognition. Whizlabs has timed mock exams that simulate the real thing.

---

## What Will Give You an Extra Edge

| Resource | Why | Time |
|---|---|---|
| **ExamTopics** (free tier) | Community-voted questions, closest to real exam style | 2-3 hours |
| **Whizlabs practice exams** (~$15) | Multiple full-length timed tests | 3-4 hours |
| **Google ML Crash Course** (free) | Fills any ML fundamentals gaps | 3-4 hours |

---

## Your Biggest Risk Areas (given your background)

You're a Platform Architect strong in infrastructure/Terraform/Kubernetes. The exam areas that might trip you up:

- **ML-specific concepts**: evaluation metrics (precision vs recall vs F1), overfitting vs underfitting, class imbalance handling -- these are pure ML theory, not infra
- **TFX pipeline component order** -- memorize this (it's in the cheat sheet)
- **Distributed training strategies** -- MirroredStrategy vs MultiWorker vs TPU -- know which for which hardware setup
- **Drift types** -- concept vs data vs skew vs attribution -- the exam LOVES these

---

## Bottom Line

Your study guide alone = **~70-75% chance of passing**. Add ExamTopics/Whizlabs practice tests + 2-3 hands-on labs = **~90%+ chance**. The hands-on labs are what turn "I read about it" into "I understand it."

---

## Repo Contents

| File | What It Is | When to Use |
|---|---|---|
| `STUDY_GUIDE.md` | Complete exam prep: 93 questions, 6 cheat sheets, study plan | Your primary study material |
| `PLATFORM_ARCHITECT_BRIDGE.md` | Maps infra/platform concepts to ML concepts | Read FIRST to accelerate learning |
| `ADDITIONAL_RESOURCES.md` | External resources, risk areas, exam strategy | Reference for supplementary study |
