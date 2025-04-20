# 🌐 GEST – Global Ethical Supply Chain Tracker

![License](https://img.shields.io/badge/license-MIT-green)
![Build](https://img.shields.io/github/workflow/status/sshyam67/gest/CI)

> AI-powered platform to monitor ethical practices in global supply chains, providing **real-time insights, risk scoring, and predictive analytics**.

---

## 📌 Table of Contents

- [Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup Instructions](#setup-instructions)
- [API Endpoints](#api-endpoints)
- [Machine Learning Model](#machine-learning-model)
- [Deployment](#deployment)
- [License](#license)
- [Contributors](#contributors)
- [Contact](#contact)

---

## 📍 Project Overview

**GEST** is an AI-based compliance tracker that monitors **labor, environmental, and governance** violations across supply chains using real-time data and ML scoring.

It empowers:
- 📈 **Companies** to monitor supply partners
- 🧑‍⚖️ **Regulators** to flag violations
- 📊 **Analysts** to predict ESG risks

---

## 🚀 Features

- ⚡ Real-time web scraping + regulatory data collection  
- 📊 Ethical scoring system across L/E/G parameters  
- 🔮 Predictive ML-based risk scoring  
- 📉 Interactive dashboards for decision-making  
- 🚨 Real-time violation alerts  
- 🔐 Secure JWT-based authentication

---

## 🏗️ Tech Stack

| Layer        | Technology                             |
|--------------|-----------------------------------------|
| Frontend     | React.js, TailwindCSS                   |
| Backend      | FastAPI, Python                         |
| Database     | PostgreSQL, MongoDB                     |
| Machine Learning | Scikit-learn, TensorFlow            |
| Web Scraping | BeautifulSoup, Requests                 |
| Auth         | JWT, OAuth2                             |
| DevOps       | Docker, GitHub Actions                  |

---

## 🛠️ Setup Instructions

```bash
# 1. Clone Repo
git clone https://github.com/sshyam67/Global-Ethical-Supply-Chain-Tracker
cd gest

# 2. Backend Setup
cd backend
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload

# 3. Frontend Setup
cd frontend
npm install
npm start

# 4. PostgreSQL Setup
docker-compose up -d db

# 5. Full App Deployment
docker-compose up --build
🔍 API Endpoints

Endpoint	Method	Description
/companies	GET	Fetch all company ethical scores
/predict	POST	Predict risk based on ESG input
/alerts	GET	Retrieve violation alerts
/token	POST	Auth with JWT
📊 Machine Learning Model
Model: Random Forest Classifier

Data: ESG + Violation Records

Accuracy: ~85%

Use Case: Predict risk score for companies in supply chain

📡 Deployment
⚙️ Docker used for containerization

🚀 GitHub Actions used for CI/CD

bash
Copy
Edit
docker build -t yourdockerhub/gest-backend:latest ./backend
docker build -t yourdockerhub/gest-frontend:latest ./frontend

docker push yourdockerhub/gest-backend:latest
docker push yourdockerhub/gest-frontend:latest
➡️ Deployed via GitHub Actions with cloud-hosted service & secure SSH.

📜 License
MIT License. Use freely, contribute openly.

🤝 Contributors
👤 Shyamkrishna – Project Lead, Full Stack Developer & Data Analyst

📞 Contact
Have questions or want to collaborate?
📧 Email: shyamkrishna9848@gmail.com
🔗 LinkedIn

⭐ If you like this project, star it & follow @sshyam67
