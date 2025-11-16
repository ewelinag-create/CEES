# CEES
CEES – Crime Escalation Early-warning System
A machine learning and NLP project analysing crime narratives to predict behavioural escalation risk

Author: Ewelina Gradwicka
Year: 2025
Status: Research Prototype

⭐ Overview

CEES (Crime Escalation Early-warning System) is an NLP-based model designed to classify short crime-style incident narratives into three escalation levels:

Low risk

Medium risk

High risk

The goal is to explore whether linguistic patterns in incident descriptions can be used to support early-warning systems in policing, safeguarding and public safety environments.

CEES integrates criminology knowledge with machine learning, bridging behavioural analysis and AI.

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

📂 Dataset file:
/data/dataset.csv

🤖 2. Models Implemented
CEES 2.0 – TF-IDF + Logistic Regression

TF-IDF vectorisation

Multinomial logistic regression

Accuracy: 0.56

Clear criminological patterns learned (e.g., threats, repeated monitoring, ex-partner contact)

📄 Results:
/results/tfidf_results.txt

CEES 3.0 – Transformer Zero-shot Classification

Model: facebook/bart-large-mnli

Zero-shot text classification

Semantic understanding of narratives

Accuracy: 0.44

Strong performance on high-risk prediction

📄 Results:
/results/bert_results.txt

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

🧪 4. Code

The full training, preprocessing and evaluation workflow is in:

📘 CEES.ipynb

Includes:

dataset loading

TF-IDF vectorisation

logistic regression classifier

zero-shot transformer pipeline

evaluation metrics and predictions

📄 5. Research Report

A complete academic-style report (PDF) describing the project:

📄 report/CEES_report.pdf

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
