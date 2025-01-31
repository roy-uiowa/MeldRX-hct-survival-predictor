# MeldRX-hct-survival-predictor
Predictive AI In Healthcare with FHIR® ---- Bringing AI and Evidence Together for SMARTer Decisions in Healthcare

# AI-Powered HCT Survival Predictor

## Overview

This project is an AI-driven healthcare application designed to predict survival probabilities for patients undergoing allogeneic Hematopoietic Cell Transplantation (HCT). Using machine learning and HL7 FHIR® standards, the app integrates patient data to provide event-free survival (EFS) predictions, offering personalized insights to assist clinicians in decision-making.

## Features

- **Survival Prediction Dashboard**: Predict event-free survival (EFS) probability using AI models.
- **FHIR® Integration**: Retrieve and store patient data securely via HL7 FHIR® APIs.
- **Explainable AI (XAI) Insights**: Utilize SHAP or similar techniques to provide interpretable predictions.
- **Equity Analysis & Bias Mitigation**: Ensure fair predictions across diverse racial and ethnic groups.
- **Personalized Recommendations**: Suggest treatment interventions to improve survival chances.

## Dataset

- **Source**: [Kaggle Competition - CIBMTR: Equity in post-HCT Survival Predictions](https://www.kaggle.com/competitions/cibmtr-equity-in-post-hct-survival-predictions)
- **Description**: The dataset contains 59 variables related to patient demographics, disease status, and treatment details.
- **Target Variable**: `efs` (Event-Free Survival) with corresponding time-to-event `efs_time`.

## Tech Stack

- **Machine Learning**: PyTorch, scikit-survival, DeepSurv, Random Survival Forests
- **Backend**: FastAPI/Django, PostgreSQL
- **FHIR® Integration**: `FHIR-Py`, HAPI-FHIR
- **Frontend**: React/Next.js
- **Deployment**: Docker, Kubernetes, AWS/GCP

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/MeldRX-hct-survival-predictor.git
   cd MeldRX-hct-survival-predictor
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Set up FHIR® connection:
   - Configure FHIR® server details in `.env` file.
4. Train the ML model:
   ```sh
   python train.py
   ```
5. Run the application:
   ```sh
   uvicorn app:main --host 0.0.0.0 --port 8000
   ```

## Usage

- Upload patient data via API or web UI.
- View survival predictions and key risk factors.
- Analyze model fairness and receive recommendations.

## Contribution

1. Fork the repository
2. Create a new feature branch (`git checkout -b feature-name`)
3. Commit changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature-name`)
5. Submit a pull request

## License

MIT License

## Contact

For questions or collaborations, reach out via [roy.uiowa at gmail.com] or open an issue in the repository.


