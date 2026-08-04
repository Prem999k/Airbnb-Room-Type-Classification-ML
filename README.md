# 🏙️ NYC Airbnb Room Type Classification ML
------------------------------------------------------
A complete **Machine Learning Web Application** that predicts the **room type** of an Airbnb listing in New York City based on listing characteristics such as location, price, availability, reviews, and host information.

The application uses a **Scikit-learn Machine Learning Pipeline** deployed with **FastAPI** as the backend and a modern responsive **HTML, CSS & JavaScript** frontend.

---

# 🌐 Live Demo
---
 https://prem999k.github.io/Airbnb-Room-Type-Classification-ML/
---

# 📖 Overview

The project predicts one of the following Airbnb room types:

* 🏠 Entire Home / Apartment
* 🚪 Private Room
* 👥 Shared Room

The prediction is generated using a trained Machine Learning classification model.

---

# ✨ Features

* Modern Responsive User Interface
* FastAPI REST API
* Machine Learning Prediction Pipeline
* Input Validation using Pydantic
* Probability Prediction
* Interactive UI
* Example Listing Generator
* API Health Check
* CORS Enabled
* Swagger API Documentation
* Production Deployment on Render

---

# 🛠 Tech Stack

## Machine Learning

* Scikit-learn
* Pandas
* NumPy
* Joblib

## Backend

* FastAPI
* Pydantic
* Uvicorn

## Frontend

* HTML5
* CSS3
* JavaScript

## Deployment

* Render
* GitHub

---

# 📂 Project Structure

```text
Airbnb-Room-Type-Classification-ML/
│
├── main.py
├── Model_Pipeline.pkl
├── index.html
├── script.js
├── style.css
├── requirements.txt
├── runtime.txt
└── nyc_airbnb_room_type_classification.ipynb
```

---

# 📊 Input Features

| Feature             | Description            |
| ------------------- | ---------------------- |
| Latitude            | Property Latitude      |
| Longitude           | Property Longitude     |
| Price               | Price per Night        |
| Minimum Nights      | Minimum Booking Nights |
| Number of Reviews   | Total Reviews          |
| Reviews Per Month   | Monthly Reviews        |
| Host Listings Count | Listings Owned by Host |
| Availability 365    | Days Available         |
| Neighbourhood Group | NYC Borough            |
| Neighbourhood       | Area Name              |

---

# 🎯 Model Output

The API returns:

```json
{
    "Predicted_room_type":"Entire home/apt",
    "Probability":[
        0.93,
        0.05,
        0.02
    ]
}
```

---

# 🚀 Installation

## Clone Repository

```bash
git clone https://github.com/Prem999k/Airbnb-Room-Type-Classification-ML.git

cd Airbnb-Room-Type-Classification-ML
```

---

## Create Virtual Environment

```bash
python -m venv venv
```

Windows

```bash
venv\Scripts\activate
```

Linux / Mac

```bash
source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Backend

```bash
uvicorn main:app --reload
```

Backend runs at

```
http://127.0.0.1:8000
```

Swagger Documentation

```
http://127.0.0.1:8000/docs
```

---

## Run Frontend

Open

```
index.html
```

or use

```
Live Server
```

---

# 🔗 API Endpoints

## GET /

Returns API status.

Response

```json
"Hello Guyss"
```

---

## POST /predict

Predicts Airbnb Room Type.

Example Request

```json
{
  "latitude":40.7484,
  "longitude":-73.9857,
  "price":120,
  "minimum_nights":2,
  "number_of_reviews":80,
  "reviews_per_month":2.1,
  "calculated_host_listings_count":1,
  "availability_365":220,
  "neighbourhood_group":"Manhattan",
  "neighbourhood":"Midtown"
}
```

---

Example Response

```json
{
  "Predicted_room_type":"Entire home/apt",
  "Probability":[
      0.95,
      0.04,
      0.01
  ]
}
```

---

# 📈 Machine Learning Workflow

```
Data Collection
        │
        ▼
Data Cleaning
        │
        ▼
Feature Engineering
        │
        ▼
Model Training
        │
        ▼
Scikit-Learn Pipeline
        │
        ▼
Model Serialization (.pkl)
        │
        ▼
FastAPI Backend
        │
        ▼
HTML/CSS/JavaScript Frontend
        │
        ▼
Prediction
```
---

# 📦 Requirements

```
fastapi
uvicorn
pandas
numpy
scikit-learn
joblib
pydantic
```

---

# 👨‍💻 Author

**Prem Kumar**

GitHub

https://github.com/Prem999k
