# 🏆 HSC Result Predictor

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![Gradio](https://img.shields.io/badge/Gradio-Interactive-green)](https://gradio.app/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

**Interactive HSC GPA predictor** built with **Python**, **Gradio**, and **Random Forest**. Predict a student's HSC GPA using personal, family, and academic information.

---

## ⚡ Features

- Predict HSC GPA based on multiple factors:
  - Gender, Age, Address
  - Family size, Parent status
  - Parents’ Education & Job
  - Tuition fee & SSC GPA
  - Relationship & Smoker status
  - Time spent with friends
- Interactive **Gradio web app**
- Output GPA clipped between **0–5**
- Easy to run locally or share online

---

## 📂 Project Structure

HSC-Result-Prediction/
│
├─ app.py # Main Gradio app code
├─ README.md # Project documentation
├─ LICENSE # MIT License
├─ student_rf_pipeline.pkl # Pre-trained Random Forest model
├─ requirements.txt # Dependencies
├─ rf_train.py # Model training script
├─ bangladesh_student_performance_2018.csv # Dataset
└─ Images/ # Screenshots or UI images


---

## ⚡ Installation

1. Clone the repository:

```bash
git clone https://github.com/mariaaktermukti/HSC-Result-Prediction.git
cd HSC-Result-Prediction
Create a virtual environment (optional):

python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate # Mac/Linux
Install dependencies:

pip install -r requirements.txt
🚀 Run the App
python app.py
Opens a browser interface via Gradio.

Provides a shareable link for external access.

## 🎯 Inputs

| Input               | Type     | Example / Options                         |
|--------------------|----------|-------------------------------------------|
| Gender             | Radio    | `M` / `F`                                 |
| Age                | Number   | `18`                                      |
| Address            | Radio    | `Urban` / `Rural`                         |
| Family Size        | Radio    | `GT3` / `LE3`                             |
| Parent Status      | Radio    | `Together` / `Apart`                      |
| Mother's Education | Slider   | `0–4`                                     |
| Father's Education | Slider   | `0–4`                                     |
| Mother's Job       | Dropdown | `At_home`, `Health`, `Other`, `Services`, `Teacher` |
| Father's Job       | Dropdown | `Teacher`, `Other`, `Services`, `Health`, `Business`, `Farmer` |
| Relationship       | Radio    | `Yes` / `No`                              |
| Smoker             | Radio    | `Yes` / `No`                              |
| Tuition Fee        | Number   | `Annual fee`                              |
| Time with Friends  | Slider   | `1–5`                                     |
| SSC Result (GPA)   | Number   | `GPA in SSC`                              |

---

🖥 Output
Predicted HSC GPA as a float between 0 to 5

Example:
Predicted HSC Result: 4.25

## 📸 Screenshots

### Full App
<img width="1919" height="1079" alt="full with app" src="https://github.com/user-attachments/assets/95106ef7-01a2-45cd-be7a-d4d17711a3c4" />

### UI Dashboard
<img width="1915" height="1079" alt="ui dashboard app" src="https://github.com/user-attachments/assets/6c813989-da98-4a80-9ce2-9b842537e88c" />


