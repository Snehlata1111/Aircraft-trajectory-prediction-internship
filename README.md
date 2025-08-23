# ✈️ Aircraft Trajectory Prediction (Internship Project)

## 📌 Project Overview
This project implements a **Long Short-Term Memory (LSTM)** deep learning model in **PyTorch** to forecast aircraft trajectories using **flight and radar datasets (50,000+ records)**.  
It focuses on **data preprocessing, feature engineering, hyperparameter tuning, and evaluation** to achieve robust predictions across multiple flight scenarios.  

The challenge is to develop a machine learning model to accurately predict three key aspects of aircraft behavior—acceleration, heading, and turn rate. Acceleration predictions indicate changes in speed, aiding in safe spacing and fuel optimization. Heading and turn rate predictions provide insights into direction and maneuvering, which are essential for collision avoidance and efficient airspace management. This model will support air traffic controllers in enhancing safety, reducing delays, and optimizing airspace use.

---

## ⚡ Features
- Processed and cleaned **50,000+ flight and radar records** for model training.  
- Built an **LSTM-based prediction model** to forecast aircraft trajectories.  
- Engineered categorical & continuous flight parameters, reducing preprocessing time by **20%**.  
- Tuned hyperparameters to improve model stability and reduce prediction variance by **15%**.  
- Evaluated predictions with **F1-score**, ensuring reliable trajectory insights.  

![Project Illustration](https://github.com/user-attachments/assets/5b7f1a09-25b4-4119-b6aa-57f6a31d6c7e)

---

## 🏗️ Tech Stack
- **Language:** Python  
- **Frameworks & Libraries:** PyTorch, NumPy, Pandas, Matplotlib, Scikit-learn  

---

## 📊 Results
- 🚀 Reduced preprocessing time by **20%**  
- 📉 Reduced prediction variance by **15%**  
- ✅ Achieved consistent forecasts across **5+ flight scenarios**  

---

## Model Training
![Training Figure](https://github.com/user-attachments/assets/fda04058-cf6e-4509-abc2-ea42531de0af)

### 🔧 Data Preparation
- Categorical variables (acceleration, heading, turn rate) → label encoded  
- Continuous variables (latitude, longitude, Cartesian coordinates, course, speed) → normalized  
- Sequences created from historical data to capture temporal dependencies  

### 🏗️ Model Architecture
- LSTM network with three output layers  
- Each output predicts a specific aircraft movement parameter: acceleration, heading, and turn rate  
- Enables simultaneous multi-target trajectory forecasting  

### 🎯 Training Process
- Loss Function: Cross-entropy loss for each output, combined into a total loss  
- Optimizer: Adam, minimizing total loss through backpropagation  
- Model trained in epochs, updating parameters after each batch of predictions  

### 📊 Evaluation
- Performance measured on a test set  
- Accuracy calculated separately for acceleration, heading, and turn rate  
- Provides insights into prediction reliability across multiple flight scenarios  

---

**About**  
Internship project applying data analytics and deep learning with LSTM models to predict aircraft trajectories using flight and radar data, focusing on preprocessing, feature engineering, and sequence modeling.
