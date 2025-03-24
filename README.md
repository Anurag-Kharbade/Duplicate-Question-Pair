# Duplicate Question Pair Detection

![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-blue)
![Flask](https://img.shields.io/badge/Backend-Flask-orange)
![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-red)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

## Overview
This project detects **duplicate question pairs** to prevent redundant content on platforms like **Quora** and **Stack Overflow**. It uses a **Random Forest Machine Learning Model** and is implemented as a **Flask web application** with a **Streamlit-based frontend**.

---

## Features
- **Random Forest Model** – Predicts duplicate questions.
- **Flask API** – Manages backend operations.
- **Streamlit UI** – User-friendly interface.
- **Dataset from Kaggle** – Pre-labeled question pairs.
- **Efficient Prediction** – Checks similarity between two questions.

---

## Installation

### Install Dependencies
```bash
pip install -r requirements.txt
```

If `requirements.txt` is unavailable, manually install:
```bash
pip install numpy pandas scikit-learn flask streamlit
```

---

## Running the Project

### Start the Flask Backend
```bash
python app.py
```
Runs the **Flask API**.

### Launch the Streamlit Frontend
```bash
streamlit run app.py
```
Opens the **web interface** for user input.

---

## Project Structure
```
│── duplicate_question_pair/
│   │── cv.pkl
│   │── model.pkl
│   │── stopwords.pkl
│── app.py
│── helper.py
│── cleaned_train.csv
│── train.csv
│── duplicate_question_pairs.ipynb
│── requirements.txt
│── Procfile.txt
│── setup.sh
│── README.md
```

---

## How It Works
1. **User Input:** Two questions are entered via the Streamlit UI.
2. **Preprocessing:** Stopwords are removed, and text is cleaned.
3. **Feature Extraction:** Questions are transformed into a machine-readable format.
4. **Model Prediction:** The trained **Random Forest model** classifies the pair as duplicate or unique.
5. **Result Display:** The UI shows the prediction.

---

## Technologies Used
- **Python**
- **Scikit-Learn (Random Forest)**
- **Flask (Backend)**
- **Streamlit (Frontend)**
- **Pandas & NumPy (Data Processing)**
