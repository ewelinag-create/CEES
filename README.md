# CEES
CEES – Crime Escalation Early-warning System
Machine Learning and NLP Project for Predicting Behavioural Escalation in Crime Narratives

Author: Ewelina Gradwicka
Year: 2025
Status: Research Prototype

Overview

CEES (Crime Escalation Early-warning System) is a Natural Language Processing (NLP) project designed to classify short crime-style narratives into three escalation levels:

Low risk

Medium risk

High risk

Its purpose is to explore whether linguistic patterns present in incident descriptions can be used to support early-warning and risk assessment systems in policing, public safety and behavioural threat contexts.
The project integrates criminological knowledge with machine learning techniques.

Project Objectives

Identify linguistic indicators associated with escalating behaviour.

Compare classical NLP methods with transformer-based models.

Evaluate the feasibility of automated narrative analysis for early intervention.

Establish a foundation for future research in AI-driven risk assessment.

1. Dataset

A synthetic pilot dataset of 29 crime-style narratives was created and manually labelled:

10 Low-risk incidents

10 Medium-risk incidents

9 High-risk incidents

The narratives simulate patterns commonly observed in real police reports, including domestic abuse, harassment, neighbour disputes, stalking, conflict escalation and antisocial behaviour.

Dataset file:
data/dataset.csv

2. Models Implemented
2.1 CEES 2.0 — TF-IDF + Logistic Regression

TF-IDF vectorisation

Multinomial logistic regression classifier

Accuracy: 0.56

Demonstrated ability to detect meaningful criminological patterns

Results file:
results/tfidf_results.txt

2.2 CEES 3.0 — Transformer Zero-shot Model

Model used: facebook/bart-large-mnli

Zero-shot text classification

Evaluates incident narratives without task-specific fine-tuning

Accuracy: 0.44

Demonstrated strong semantic understanding of high-risk patterns

Results file:
results/bert_results.txt

3. Key Findings
High-risk indicators

Words frequently associated with high-risk incidents included:
partner, ex, victim, threats, restraining, weapons, followed, consecutive, monitoring.

Medium-risk indicators

neighbours, arguing, injuries, returning, night, customer.

Low-risk indicators

parking, noise, construction, drivers, teenagers, flat.

These patterns correspond with criminological theories related to coercive control, repeat victimisation, dispute escalation and behavioural threat assessment.

4. Code

All preprocessing, modelling and evaluation steps are included in the notebook:
CEES.ipynb

The notebook contains:

Text preprocessing

TF-IDF feature extraction

Logistic regression classifier

Zero-shot transformer pipeline

Evaluation and predictions

5. Research Report

A full academic-style project report is included in PDF form:
report/CEES_report.pdf

6. Future Work

Planned future improvements include:

Expansion to a much larger dataset

Fine-tuning transformer-based models for domain-specific classification

Integration of contextual metadata (relationship type, history, temporal variables)

Implementation of explainable AI techniques

Development of a deployment-ready API

7. Technologies Used

Python

Scikit-learn

HuggingFace Transformers

Pandas

NumPy

Google Colab

TF-IDF Vectorisation

Logistic Regression

Zero-shot Classification

8. About the Author

I am a Criminology student with a strong interest in Artificial Intelligence applications in public safety, behavioural analysis and risk prediction. CEES combines the theoretical foundations of criminology with modern NLP techniques to explore how AI can support early intervention and evidence-based decision-making.

9. Contact

For collaboration or feedback:
Email: ewelina.gradwicka@gmail.com
