GEST - Global Ethical Supply Chain Tracker

📌 Project Overview

GEST (Global Ethical Supply Chain Tracker) is an AI-powered platform that provides real-time monitoring, scoring, and predictive analysis of ethical practices in supply chains. It tracks corporate compliance with labor, environmental, and governance standards by aggregating data from multiple sources.

🚀 Features

Real-time data collection from regulatory reports, company disclosures, and web scraping.

Ethical Score Calculation based on labor, environmental, and governance factors.

AI-based risk prediction using machine learning.

Interactive dashboards for companies and regulators.

Real-time alerts for supply chain violations.

Secure authentication & authorization using JWT.

🏗️ Tech Stack

Component

Technology Used

Frontend

React.js, TailwindCSS

Backend

FastAPI, Python

Database

PostgreSQL, MongoDB

Machine Learning

Scikit-learn, TensorFlow

Web Scraping

BeautifulSoup, Requests

Authentication

JWT, OAuth2

Deployment

Docker, GitHub Actions

🛠️ Setup Instructions

1️⃣ Clone the Repository

 git clone https://github.com/sshyam67/Global-Ethical-Supply-Chain-Tracker
 cd gest

2️⃣ Backend Setup (FastAPI)

 cd backend
 python -m venv venv
 source venv/bin/activate  # (Windows: venv\Scripts\activate)
 pip install -r requirements.txt
 uvicorn main:app --reload

3️⃣ Frontend Setup (React.js)

 cd frontend
 npm install
 npm start

4️⃣ Database Setup (PostgreSQL)

 docker-compose up -d db

5️⃣ Running the Full Application

 docker-compose up --build

🔍 API Endpoints

Endpoint

Method

Description

/companies

GET

Fetch all company ethical scores

/predict

POST

Predict ethical risk of a company

/alerts

GET

Fetch real-time alerts

/token

POST

User authentication

📊 Machine Learning Model

Algorithm Used: Random Forest Classifier

Training Data: Labor, environmental, governance scores with violation records.

Accuracy: ~85%

📡 Deployment

This project uses Docker & GitHub Actions for continuous integration and deployment.

Build & Push Docker Images:

 docker build -t yourdockerhub/gest-backend:latest ./backend
 docker build -t yourdockerhub/gest-frontend:latest ./frontend
 docker push yourdockerhub/gest-backend:latest
 docker push yourdockerhub/gest-frontend:latest

Deploy via SSH (GitHub Actions)

GitHub Actions workflow automates building, pushing, and deploying to a cloud server.

📜 License

This project is open-source under the MIT License.

🤝 Contributors

Shyamkrishna - Project Lead


📞 Contact

For inquiries, reach out at: shyamkrishna9848@gmail.com
