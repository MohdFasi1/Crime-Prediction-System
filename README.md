
<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg" width="80" />
  <img src="https://upload.wikimedia.org/wikipedia/commons/2/2d/Tensorflow_logo.svg" width="80" />
  <h2 align="center">🧠 Crime Prediction System using biConvLSTM</h2>
  <p align="center"><i>Predicting crime patterns using deep learning and spatiotemporal data</i></p>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/python-3.10.9-blue.svg" />
  <img src="https://img.shields.io/badge/tensorflow-2.19.0-orange.svg?logo=tensorflow" />
  <img src="https://img.shields.io/badge/status-deployed-brightgreen" />
  <img src="https://img.shields.io/badge/License-MIT-green.svg" />
</p>

---

## 📌 Overview

This project leverages a **bi-directional Convolutional LSTM (biConvLSTM)** model to forecast future crime occurrences based on historical spatial and temporal data. It's designed to help law enforcement and researchers visualize and analyze crime trends with predictive accuracy.

---

## 🔍 Features

- 🔄 **biConvLSTM** architecture for spatiotemporal pattern learning
- 📍 Geospatial and temporal crime trend prediction
- 🚨 Predicts crime probability based on location, date, time, and crime type.
- 🏙️ Focused on city-wise data within Hyderabad.
- 📊 Trained on a robust dataset with over 40,000 crime records.
- 🌐 Web-based interface using Flask
- 

---

## ⚙️ Tech Stack

| Component     | Technology Used                          |
| ------------- | ---------------------------------------- |
| Model         | biConvLSTM (TensorFlow + Keras)          |
| Backend       | Flask (Python 3.10.9)                    |
| Data Handling | Pandas, NumPy                            |
| Visualization | Matplotlib, Seaborn                      |

---

## 🧪 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/crime-prediction-system.git
cd crime-prediction-system
```

### 2. Create a Virtual Environment

```bash
python3.10 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run Locally

```bash
python app.py
```

Visit: [http://localhost:5000](http://localhost:5000)

> ⚠️ **Important:** This project requires **Python 3.10.9** and **TensorFlow 2.13.0**. Newer versions may not be compatible.

---

## 🔐 Environment Variables

Create a `.env` file in the root of your project:

```
apiKey=your_api_key
authDomain=your_auth_domain
projectId=your_project_id
storageBucket=your_storage_bucket
messagingSenderId=your_messaging_sender_id
appId=your_app_id
measurementId=your_measurement_id
```

---

## 🧾 Requirements

Sample `requirements.txt` includes:

```txt
python-dotenv==1.1.0
tensorflow==2.13.0
pandas==2.3.0
numpy==1.24.4
scikit-learn==1.3.2
matplotlib==3.7.1
seaborn==0.13.2
gunicorn==23.0.0
flask==2.3.3
```

> ⚠️ Avoid `numpy>=2` for now — some libraries may crash.

---

## 📁 Project Structure

```
├── app.py
├── model
|   ├── dataPreprocess.ipynb
|   ├── crime_detection_model_Generator.ipynb
|   ├── crime_data.csv
|   ├── conv_bilstm_autoencoder.h5
|   └── ...
├── templates/
│   ├── index.html
│   ├── details.html
│   └── ...
├── static/
│   ├── styles.css
│   ├── *.jpg
│   └── ...
├── .env
├── .python-version
├── requirements.txt
└── README.md
```
---


## 👨‍💻 Author

Developed by [Mohd Fasi Uddin](https://github.com/MohdFasi1)

---

## 📄 License

This project is under the [MIT License](LICENSE).
