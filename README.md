# 🏙️ NYC Airbnb Room Type Predictor

A machine learning web application that predicts the **Airbnb room type** for a New York City listing based on listing and location features.

The project combines a **scikit-learn machine learning pipeline**, **FastAPI backend**, and a responsive **HTML/CSS/JavaScript frontend**.

---

## 🚀 Features

- 🤖 Machine learning-based room type prediction
- ⚡ FastAPI backend for serving predictions
- 🌐 Interactive web frontend
- 🔐 CORS-enabled API for frontend/backend communication
- 📊 Uses NYC Airbnb listing features such as price, reviews, availability, and location
- 🧩 Pre-trained model pipeline loaded with `joblib`
- 📖 FastAPI interactive API documentation through Swagger UI

---

## 🛠️ Tech Stack

### Backend
- Python
- FastAPI
- Pydantic
- Uvicorn
- Pandas
- Joblib

### Machine Learning
- Scikit-learn
- Pre-trained classification pipeline
- Decision Tree / Random Forest-based estimators

### Frontend
- HTML5
- CSS3
- JavaScript

---

## 📋 Input Features

The prediction API uses features including:

- Latitude
- Longitude
- Price
- Minimum nights
- Number of reviews
- Reviews per month
- Calculated host listings count
- Availability over 365 days
- Neighbourhood group
- Neighbourhood

The model uses these listing attributes to predict the room type.

---

## 📁 Project Structure

```text
NYC-Airbnb-Room-Type-Predictor/
│
├── frontend/
│   ├── index.html
│   ├── script.js
│   ├── style.css
│   └── the_build_line_guide.html
│
├── main.py
├── Model_Pipeline.pkl
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/sritamapaul1042-max/NYC-Airbnb-Room-Type-Predictor.git
cd NYC-Airbnb-Room-Type-Predictor
```

### 2. Create a virtual environment

```bash
python3 -m venv venv
```

### 3. Activate the virtual environment

macOS / Linux:

```bash
source venv/bin/activate
```

Windows:

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

If needed, the main backend dependencies are:

```bash
pip install fastapi uvicorn pydantic pandas joblib scikit-learn
```

---

## ▶️ Run the Backend

From the project root:

```bash
uvicorn main:app --reload
```

The API will be available at:

```text
http://127.0.0.1:8000
```

### API Documentation

Open:

```text
http://127.0.0.1:8000/docs
```

This opens FastAPI's interactive Swagger documentation.

---

## 🌐 Run the Frontend

Open `frontend/index.html` with **VS Code Live Server**.

The frontend will normally be available at:

```text
http://127.0.0.1:5500
```

Keep the FastAPI backend running while using the frontend.

---

## 🔄 How It Works

```text
User enters listing details
          ↓
      Frontend
   (HTML + JS + CSS)
          ↓
    FastAPI REST API
          ↓
   Input validation
      (Pydantic)
          ↓
 Model_Pipeline.pkl
          ↓
 Room type prediction
          ↓
 Prediction displayed
      on frontend
```

---

## 🧠 Machine Learning Model

The project uses a pre-trained scikit-learn pipeline stored in:

```text
Model_Pipeline.pkl
```

The pipeline handles the model's preprocessing and prediction workflow so that the API can receive listing information and return a room type prediction.

---

## 🔌 Backend API

The FastAPI application exposes a prediction endpoint for receiving listing features and returning the model's prediction.

You can inspect and test the available endpoints through:

```text
http://127.0.0.1:8000/docs
```

---

## 📸 Screenshots

Add screenshots of the working application here to make the repository easier to understand for recruiters and other developers.

Example:

```markdown
![NYC Airbnb Predictor](screenshots/homepage.png)
```

---

## 🎯 Project Goals

This project demonstrates practical experience with:

- Machine learning model deployment
- REST API development
- FastAPI
- Pydantic data validation
- Frontend and backend integration
- Model serialization with Joblib
- Git and GitHub
- End-to-end ML application development

---

## 🔮 Future Improvements

- Deploy the FastAPI backend to a cloud platform
- Deploy the frontend publicly
- Add model performance metrics
- Add prediction confidence/probabilities
- Improve input validation and error messages
- Add automated tests
- Add Docker support
- Add more visual analytics for NYC Airbnb listings

---

## 👩‍💻 Author

**Sritama Paul**

GitHub: [sritamapaul1042-max](https://github.com/sritamapaul1042-max)

---

## ⭐ If you found this project useful

Feel free to star the repository and explore the code!
