# Machine Learning Pose Detection Framework for Suspicious Activity Recognition

## 🧠 Overview
This research project centers on real-time detection of suspicious human activity using machine learning and pose estimation. Suspicious behavior often involves unusual or erratic body movements, which are challenging to detect with traditional rule-based surveillance systems due to computational limitations and lack of adaptability.

## 🎯 Objective
To design a computationally efficient, real-time AI framework that improves surveillance systems by:
1. Detecting anomalous or “suspicious” movements using pose estimation.
2. Classifying specific types of suspicious activities for further action or alerting.

## 🧩 Framework Components

| Component | Description |
|-----------|-------------|
| **Pose Estimation** | Used MediaPipe’s BlazePose model to extract complete 3D body joint information (x, y, z coordinates). |
| **Feature Engineering** | Custom geometric features created from pose coordinates for improved classification performance. |
| **Primary Model** | Binary classifier (e.g., Random Forest) determines whether an activity is suspicious or not. |
| **Secondary Model** | Activity classifier (e.g., XGBoost) identifies the type of suspicious activity if flagged in the primary step. |
| **Alert Mechanism** | Triggers real-time alerts on detecting specific risky movements. |

## 📊 Dataset

- **Size:** ~1900 surveillance video clips.
- **Classes:** 13 activity classes (normal & suspicious activities).
- **Source:** Real-world annotated surveillance footage.

## 🧪 Algorithms Evaluated

| Task | Models Tested | Best Performer |
|------|---------------|----------------|
| **Primary Classification** (Suspicious / Not Suspicious) | Random Forest, LightGBM, XGBoost, DNN | **Random Forest — 93% Accuracy** |
| **Secondary Classification** (Activity Recognition) | Random Forest, LightGBM, XGBoost, DNN | **XGBoost — 70% Accuracy** |

## 🛠️ Tools & Technologies

- **Pose Estimation:** MediaPipe BlazePose  
- **ML Algorithms:** Random Forest, XGBoost, LightGBM, Deep Neural Networks  
- **Programming:** Python (NumPy, Pandas, scikit-learn), TensorFlow/Keras  
- **Visualization:** Matplotlib, Seaborn  

## 🔍 Impact & Applications

The proposed framework can be deployed in:
- CCTV-based surveillance systems  
- Public safety and monitoring infrastructure  
- Automated anomaly detection for security companies  
- Real-time alerting for critical facilities and smart city applications  

