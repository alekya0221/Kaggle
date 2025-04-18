#  Acumen: ML Insights Dashboard

Acumen is a multimodal, ML-powered insights platform built with Streamlit and MLflow. It supports structured predictions, SHAP explainability, CSV batch processing, and drag-and-drop uploads for PDFs, MP3s, and PNGs.

---

##  Quickstart (with Docker Compose)

### 1.  Install Docker
- [Download Docker Desktop](https://docs.docker.com/get-docker) for your OS.

### 2.  Clone or unzip the project folder
Make sure these files are inside the folder:

```
Acumen/
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── app.py
├── train.py
└── README.md
```

### 3.  Build and launch
From the root project folder:

```bash
docker-compose up --build
```

### 4.  Open in browser
- Streamlit App → [http://localhost:8501](http://localhost:8501)
- MLflow UI → [http://localhost:5000](http://localhost:5000)

---

##  Features

| Feature                     | Description                                     |
|----------------------------|-------------------------------------------------|
|  Slider-based Inputs      | Real-time feature tuning                        |
|  Class Prediction         | Predict label + show confidence levels          |
|  SHAP Explainability      | Feature contribution visualization              |
|  CSV Batch Upload         | Bulk predictions from uploaded CSV              |
|  MP3, PDF, PNG Support    | Drag-and-drop multimodal data ingestion         |
|  Dockerized               | Works out-of-the-box anywhere with Docker       |

---

##  Project Structure

```
Acumen/
├── app.py                  # Streamlit app
├── train.py                # Model training + MLflow logging
├── requirements.txt        # All dependencies
├── Dockerfile              # Docker build for app container
├── docker-compose.yml      # Multi-container (App + MLflow)
└── mlruns/                 # Auto-created for MLflow logs
```

---

##  Contributions
Pull requests welcome! Want to extend Acumen with PDF summarization, Whisper+GPT Q&A, or MongoDB storage? Fork and go wild!

---

##  Contact
Made by Alekya Seerapu · Reach out at alekya0221@gmail.com

---

> Acumen: Insights made simple. Predictions made explainable. 
