# 🥛 Dairy Quality Prediction

A **full-stack AI/ML application** for predicting milk quality using **machine learning** models and a modern **React** frontend with a **Flask** backend.  
This project integrates **Random Forest** and **SVM** models with **stacking (Logistic Regression)** to improve prediction accuracy.

---

## 📌 Features

- **Frontend:** React-based, responsive UI for input and result visualization.
- **Backend:** Flask API for model inference and data handling.
- **Machine Learning:**
  - Random Forest (`random_forest_model.pkl`)
  - Support Vector Machine (`svm_model.pkl`)
  - Stacking with Logistic Regression for better accuracy
- **Data:** Trained on milk quality dataset (`milknew.csv`).
- **Serialization:** Models stored using **Pickle** for quick loading.
- **Prediction Display:** Real-time prediction results on the UI.

---

## 🛠 Tech Stack

**Frontend**
- React
- Tailwind CSS (if used)
- Axios (for API calls)

**Backend**
- Python
- Flask
- scikit-learn
- Pandas
- Pickle

---

## 📂 Project Structure


## File Structure
### Frontend

```
┌── .eslintrc.json
├── .gitignore
├── CHANGELOG.md
├── LICENSE.md
├── next.config.js
├── package.json
├── README.md
├── public
└── src
	├── components
	├── contexts
	├── guards
	├── hocs
	├── hooks
	├── layouts
	├── sections
	├── theme
	├── utils
	└── pages
		├── 404.js
		├── _app.js
		├── _document.js
		├── account.js
		├── companies.js
		├── customers.js
		├── index.js
		├── products.js
		└── settings.js
		└──  auth
			├── login.js
			└── register.js
```
### Backend 

```
/server # Backend API logic (if separated)
  ├── /pyenv # Virtual environment
  ├── /templates # HTML templates (Flask rendering)
  ├── app.py # Flask application entry point
  ├── model.py # Model training, loading, and prediction logic
  ├── milknew.csv # Dataset for training/testing
  ├── random_forest_model.pkl# Trained Random Forest model
  ├── svm_model.pkl # Trained SVM model
  ├── requirements.txt # Python dependencies
└── 

```

---

## 🚀 Getting Started

### 1️⃣ Clone the repository
```bash
git clone [https://github.com/Atharva0920/dairy-quality-prediction.git](https://github.com/Atharva0920/Milk-Quality-Prediction.git)
cd Milk-Quality-Prediction



Frontend Setup -> 

cd client
npm install
npm start

Frontend will run at: http://localhost:3000/

Backend Setup -> 

cd server
python -m venv pyenv
source pyenv/bin/activate   # On Windows: pyenv\Scripts\activate
pip install -r requirements.txt
python app.py

```

📊 Model Workflow

- Data Preprocessing: Clean and prepare milknew.csv.

- Model Training:

- Train Random Forest and SVM models.

- Use stacking with Logistic Regression for final prediction.

- Pickle Serialization: Save models as .pkl files.

- Prediction API: Load .pkl files in model.py and expose via Flask endpoints.

- UI Integration: React frontend calls API to display predictions.

📷 Screenshots



📈 Accuracy Improvements

- Used stacking to combine predictions from Random Forest and SVM.

- Logistic Regression meta-model improved accuracy by leveraging strengths of both models.
