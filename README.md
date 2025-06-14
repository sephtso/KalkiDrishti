# KalkiDrishti
Crime prediction system using ML (KNN, Decision Tree, Random Forest) on Guwahati police data with role-based access and visual analytics.
👁️ KalkiDrishti – Predicting Crimes Using Machine Learning



![logo(2) png](https://github.com/user-attachments/assets/9c49527b-e284-4f30-907d-9f6f17c1bab2)



**KalkiDrishti** (क्ल्कि दृष्टि) is an intelligent crime prediction system that uses machine learning to analyze temporal and geospatial crime data from the city of Guwahati, India. It forecasts likely criminal activities, identifies crime hotspots, and enables role-based access for civilians and law enforcement to collaborate in reporting and analyzing incidents.  

Developed as part of a final-year B.Tech project at Assam Down Town University, this solution leverages classification algorithms such as **K-Nearest Neighbors (KNN)**, **Decision Trees**, and **Random Forests** for predicting crime categories based on **timestamp**, **location**, and **IPC sections**.

---

📌 Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [System Architecture](#system-architecture)
- [Dataset](#dataset)
- [Machine Learning Models](#machine-learning-models)
- [Setup & Installation](#setup--installation)
- [Testing](#testing)
- [Screenshots](#screenshots)
- [Future Scope](#future-scope)
- [Contributors](#contributors)
- [License](#license)

---

## 🚀 Features

- 🔐 Role-based login for civilians and police officers
- 📝 Civilians can report crimes with a timestamp and location
- 📂 Officers access structured crime data through a secure dashboard
- 📊 Crime prediction based on ML algorithms
- 🧠 Multi-class classification and hotspot forecasting
- 🌍 Visual analytics using Leaflet maps and interactive charts

---

🎥 Demo



🛠️ Technologies Used

🔙 Backend (ML & API)
- **Python 3.6.5**
- **Anaconda Navigator**
- **Scikit-learn** (KNN, Decision Tree, Random Forest)
- **Pandas, NumPy, Geopy**

🌐 Frontend
- **React.js + Next.js**
- **TypeScript**
- **Tailwind CSS**
- **Leaflet.js (Map visualization)**

### 🔐 Auth & Infra
- **bcryptjs** (for password hashing)
- **Zod** (for input validation)

---

## 🧠 System Architecture

```plaintext
+------------------+          +------------------+          +----------------------+
|  Civilian Portal |   -->    |  Flask/Django API|   -->    |  Crime Classifier    |
+------------------+          +------------------+          +----------------------+
         ^                                                           |
         |                                                           v
+------------------+                                        +----------------------+
| Police Dashboard |   <--    Real-Time Reports             |  Random Forest Model |
+------------------+                                        +----------------------+

