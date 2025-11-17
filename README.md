CEES – Crime Escalation Early-warning System

A proof-of-concept machine learning project for detecting escalation risk in short crime-related narratives.

⭐ Overview

CEES is an exploratory NLP + machine learning project designed to analyse short police-style incident narratives and classify them into three escalation levels:

low risk

medium risk

high risk

The project compares two approaches:

Traditional ML: TF-IDF + Logistic Regression (CEES 2.0)

Transformer model: Zero-shot classification using BART-large MNLI (CEES 3.0)

The goal is to explore whether AI can support early identification of escalating behaviour in domains such as interpersonal conflict, domestic abuse, harassment and neighbour disputes.

📁 Project Structure
CEES/
│
├── data/
│   └── dataset.csv
│
├── results/
│   ├── tfidf_results.txt
│   └── bert_results.txt
│
├── report/
│   └── CEES report.pdf
│
├── CEES_project.ipynb
├── requirements.txt
└── README.md

📓 Notebook

Kliknij tutaj, aby uruchomić pełny notebook w Google Colab:

🔍 Dataset

The dataset contains 29 short incident descriptions, each manually labelled as:

low

medium

high

It is a synthetic but criminologically realistic dataset designed for experimental research.

📄 Dataset:
data/dataset.csv

🤖 Models Used
CEES 2.0 – TF-IDF + Logistic Regression

Accuracy: 0.78

Clear linguistic separation between risk levels

Best performance on this small dataset

📄 Wyniki:
tfidf_results.txt

CEES 3.0 – Zero-shot Transformer (BART-large MNLI)

Accuracy: 0.33

Expected lower performance due to zero training on dataset

Useful as baseline for semantic similarity

📄 Wyniki:
bert_results.txt

📊 Key Findings

TF-IDF + Logistic Regression significantly outperforms the transformer zero-shot classifier.

High-risk narratives are strongly associated with:

stalking precursors

repeated monitoring

coercive control

harassment

property damage

ex-partner behaviour

Medium and low risk categories show distinct linguistic patterns.

The system successfully captures criminological escalation indicators.

🛠 How to run

Pobierz repozytorium:

git clone https://github.com/ewelinag-create/CEES.git


Zainstaluj wymagane biblioteki:

pip install -r requirements.txt


Otwórz notebook:

CEES_project.ipynb


Uruchom wszystkie komórki, aby odtworzyć:

CEES 2.0 (TF-IDF + LR)

CEES 3.0 (Zero-shot BART)

⚠️ Limitations

Very small dataset (29 samples)

Labels simplified (low/medium/high)

Not a production tool

No external validation

Results not generalisable to policing or safeguarding contexts

This is a research prototype, not a decision-making system.

🧭 Ethics & Bias

AI for policing must be developed with extreme caution.

Potential risks include:

dataset bias

reporting disparities

misclassification of vulnerable groups

model overconfidence

CEES should be used only as decision support, under full human oversight.

📘 Technologies

Python

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

HuggingFace Transformers

BART-large MNLI

👩‍🎓 About the Author

Ewelina Gradwicka
BSc Criminology (London Metropolitan University)
Combining criminology, behavioural analysis and applied machine learning to develop AI tools for violence prevention, escalation detection and public safety.

📧 ewelina.gradwicka@gmail.com

🔗 GitHub: ewelinag-create
