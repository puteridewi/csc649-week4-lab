# Tech Stack Evaluation

## Project
Machine Learning-based Food Waste Prevention System Through Predictive Spoilage Risk Assessment and Inventory Prioritization

## Requirements that drive the decision
List 3 to 5 requirements from your own docs/requirements.md. Include at
least 2 non-functional requirements.
- FR1 : The system shall allow users to record a food name, purchase date, storage type, and initial freshness status.
- FR2 : The system shall display saved grocery items and their recorded details.
- FR3 : The system shall generate a spoilage-related prediction for an eligible item using the selected trained model and supported input features.
- NFR1 : In the defined test environment, at least 95% of valid prediction requests shall complete within 2 seconds.
- NFR2 : The project shall evaluate whether the selected classification model reaches the proposed target of at least 85% accuracy on held-out data; this is a target, not an achieved result.

## Options
- Option A: Flutter + Firebase + Python FastAPI
- Option B: React Native + Supabase + Python FastAPI
- Option C: Python Flask + SQLite + Scikit-learn

## Decision matrix
Weight: how important the criterion is for YOUR project (1 = low, 5 = high).
Score: how well each option does (1 = poor, 5 = excellent).
Weighted score = weight x score. Add them up for each option.

| Criterion                          | Weight | A score | B score | C score |
|------------------------------------|--------|---------|---------|---------|
| Fits my requirements               |    5    |     5    |    5     |    3     |
| Skills I already have              |   4     |     3    |     3    |     4    |
| Time to build before my deadline   |    5    |     3    |     3    |     4    |
| Free hosting and tools             |    4    |    4     |    4     |     5    |
| Performance and security needs     |    4    |     4    |     4    |     3    |
| Room to grow later                 |    3    |     5    |     5    |     3    |
| **Total (weighted)**               |        |    99     |     99    |     92    |

## Decision record

- **Context:** The project aims to develop a mobile-based food waste prevention system that uses machine learning to predict food spoilage risks and prioritize grocery inventory. The main constraints are development time, programming skills, project requirements and development cost.

- **Decision:** Select Option A – Flutter, Firebase and Python FastAPI, with Scikit-learn for machine learning implementation.

- **Reasons:**
  1. Flutter supports cross-platform mobile application development, matching the project's preferred platform.
  2. Python FastAPI and Scikit-learn support integration of machine learning models such as Random Forest and XGBoost for spoilage risk prediction.
  3. Firebase provides cloud database services for managing grocery inventory information.

- **Consequences:** The selected stack provides a dedicated mobile application, cloud-based inventory management and machine learning integration. However, integrating Flutter, Firebase and FastAPI requires additional development effort and knowledge of multiple technologies.

- **Risks and next review:** Potential risks include integration difficulties, limited free-tier cloud resources, internet connectivity dependency and insufficient dataset quality for accurate predictions. The decision will be reviewed if Flutter development exceeds the available timeline, integration becomes too complex, or another technology stack provides a more suitable solution.