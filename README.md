# 🩺 Healthcare Chatbot 

An intelligent **Healthcare Chatbot** that predicts possible diseases based on user symptoms and provides descriptions, precautions, and confidence scores.
The system uses a **Random Forest Classifier** along with symptom extraction techniques such as synonym mapping and fuzzy matching to improve accuracy and user experience.

---

## 🚀 Features

* Predicts diseases based on user symptoms
* Uses **Machine Learning (Random Forest)** for classification
* Accepts **natural language symptom input**
* Supports:

  * Synonym detection (e.g., *tummy pain → stomach_pain*)
  * Typo handling using fuzzy matching
* Interactive chatbot with guided follow-up questions
* Provides:

  * Disease prediction with confidence %
  * Disease description
  * Suggested precautions
* Includes empathetic health messages for better user experience

---

## 🧠 Machine Learning Details

* Algorithm: **RandomForestClassifier**
* Data preprocessing:

  * Duplicate column cleaning
  * Label encoding for target values
* Train-test split: 67% training / 33% testing
* Probability-based prediction for confidence score

---

## 📂 Project Structure

```
Healthcare-Chatbot/
│
├── chatbot.py
├── Data/
│   ├── Training.csv
│   └── Testing.csv
│
├── MasterData/
│   ├── symptom_Description.csv
│   ├── symptom_severity.csv
│   └── symptom_precaution.csv
│
└── README.md
```

---

## ⚙️ Installation

1. Clone the repository

```bash
git clone https://github.com/your-username/Healthcare-Chatbot.git
cd Healthcare-Chatbot
```

2. Install required libraries

```bash
pip install pandas numpy scikit-learn
```

---

## ▶️ How to Run

```bash
python chatbot.py
```

The chatbot will:

* Ask for basic details (name, age, gender)
* Accept symptom description
* Ask follow-up questions
* Predict the disease and provide recommendations

---

## 📝 Example Input

```
I have fever and body pain for 3 days
```

**Output:**

* Predicted disease
* Confidence level
* Description
* Precautions

---

## 🔍 Symptom Intelligence

The chatbot improves input understanding using:

| Method           | Example                     |
| ---------------- | --------------------------- |
| Synonym Mapping  | "belly pain" → stomach_pain |
| Fuzzy Matching   | "feaver" → fever            |
| Phrase Detection | "shortness of breath"       |

---

## ⚠️ Disclaimer

This project is for **educational purposes only** and should **not be used as a medical diagnosis tool**. Always consult a qualified healthcare professional for medical advice.

---

## 📈 Future Improvements

* Web or mobile interface
* Deep learning model
* Voice input support
* API deployment (Flask/FastAPI)
* Integration with hospital databases

---

Give it a **star** on GitHub and feel free to contribute!
