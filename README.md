# CEES
CEES – Crime Escalation Early-warning System
A machine learning and NLP project analysing crime narratives to predict behavioural escalation risk

Author: Ewelina Gradwicka
Year: 2025
Status: Research Prototype

⭐ Overview 
## **Overview**

CEES (Crime Escalation Early-warning System) is an NLP-based model designed to classify short crime-style incident narratives into three escalation levels:

Low risk

Medium risk

High risk

The goal is to explore whether linguistic patterns in incident descriptions can be used to support early-warning systems in policing, safeguarding and public safety environments.

CEES integrates criminology knowledge with machine learning, bridging behavioural analysis and AI.
## How to run

1. Clone this repository or download it as a ZIP:
   ```bash
   git clone https://github.com/ewelinag-create/CEES.git
2. Install the required Python packages (see `requirements.txt`):
   ```bash
   pip install -r requirements.txt
3. Open the notebook CEES_project.ipynb in Jupyter or Google Colab
4. Run all cells to reproduce the results for:

CEES 2.0 – TF-IDF + Logistic Regression

CEES 3.0 – zero-shot transformer classifier (BART-large MNLI)

### Notebook

You can explore and run the full CEES notebook here:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ewelinag-create/CEES/blob/main/CEES_project.ipynb)


⭐ Project Goals

Identify textual patterns associated with conflict escalation

Compare classical NLP (TF-IDF + logistic regression) with transformer-based models

Demonstrate the feasibility of narrative analysis for risk assessment

Build a foundation for future AI tools supporting early intervention

🔍 1. Dataset

A synthetic pilot dataset of 29 crime-style narratives, labelled as:

10 Low risk

10 Medium risk

9 High risk

Narratives cover:
domestic abuse, neighbour disputes, harassment, stalking, antisocial behaviour and general community conflicts.

📂 Dataset file: [data/dataset.csv](data/dataset.csv)

🤖 2. Models Implemented
CEES 2.0 – TF-IDF + Logistic Regression

TF-IDF vectorisation

Multinomial logistic regression

Accuracy: 0.78

Clear criminological patterns learned (e.g., threats, repeated monitoring, ex-partner contact)

📄 Results (TF-IDF): [results/tfidf_results.txt](results/tfidf_results.txt)

CEES 3.0 – Transformer Zero-shot Classification

Model: facebook/bart-large-mnli

Zero-shot text classification

Semantic understanding of narratives

Accuracy: 0.33

Strong performance on high-risk prediction

📄 Results (BERT zero-shot): [results/bert_results.txt](results/bert_results.txt)

📈 3. Key Findings
🔥 High-risk language indicators:

partner, ex, victim

threats, restraining, weapons

followed, consecutive, monitoring

🔥 Medium-risk indicators:

neighbours, arguing, injuries

returning, night, customer

🔥 Low-risk indicators:

parking, noise, construction

drivers, teenagers

These patterns align with criminological theory:

coercive control

repeat victimisation

conflict escalation models


## Limitations

CEES is a **pilot proof-of-concept**, not a production system.  
Key limitations:

- Very small, synthetic dataset (29 short narratives).  
- Labels (low / medium / high) are simplified and do not capture the full complexity of real-world risk assessment.  
- No external validation set or cross-domain testing.  
- Models are trained and evaluated on the same narrow context.

Results therefore **cannot be generalised** to operational policing or safeguarding.  
The project is intended as an exploratory research prototype showing how NLP and machine learning could support criminological thinking about escalation.

## Ethics and Bias

Any AI system used in policing, safeguarding or risk assessment must be treated with extreme caution.

Potential sources of bias include:

- unrepresentative or historically biased data,  
- differences in reporting and enforcement across communities,  
- model overconfidence in ambiguous or borderline cases.

Tools like CEES should only be used as **decision support**, under human supervision, and never as the sole basis for action.  
Transparency, accountability and continuous auditing are essential for any real-world deployment.

🧪 4. Code

The full training, preprocessing and evaluation workflow is in:

📘 Notebook: [CEES_project.ipynb](CEES_project.ipynb)

Includes:

dataset loading

TF-IDF vectorisation

logistic regression classifier

zero-shot transformer pipeline

evaluation metrics and predictions

📄 5. Research Report

A complete academic-style report (PDF) describing the project:

📄 [Download full report (PDF)](report/CEES%20report.pdf)


🚀 6. Future Work

Expand dataset (1000+ narratives)

Fine-tune transformer models (BERT, RoBERTa, DeBERTa)

Add contextual metadata (relationship, history, timestamps)

Implement explainable AI (SHAP, LIME)

Develop a deployment-ready API for real-time risk scoring

🧩 7. Technologies Used

Python

Scikit-learn

HuggingFace Transformers

Pandas / NumPy

Google Colab

TF-IDF Vectorisation

Logistic Regression

Zero-shot Classification

👩‍💻 8. About the Author

I am a Criminology student passionate about applying Artificial Intelligence to behavioural risk prediction, conflict escalation and public safety challenges. This project combines criminology and machine learning to explore new ways AI can support early intervention and evidence-based decision-making.

⭐ 9. Contact

If you would like to collaborate, discuss the research or provide feedback:
Email: ewelina.gradwicka@gmail.com
