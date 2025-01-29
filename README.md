# 🌟 Fitness Tracker Data Analysis & Prediction

Welcome to the **Fitness Tracker Data Analysis & Prediction** project! This project focuses on analyzing fitness tracking data and predicting **Calories Burned** using **Deep Learning**. 

## 📚 Overview

We process a **synthetic fitness dataset** that includes various health and exercise-related parameters. We clean and preprocess the data, apply feature engineering, and train a **Neural Network** to predict the number of calories burned.

## 📊 Dataset Details

The dataset contains information on:
- **Demographics:** Age, Gender, Weight, Height
- **Heart Rate Metrics:** Max BPM, Average BPM, Resting BPM
- **Fitness Stats:** Workout Duration, Frequency, Experience Level
- **Health Factors:** Fat Percentage, BMI, Water Intake
- **Workout Type**
- **Target Variable:** Calories Burned

## 🎨 Data Preprocessing

To ensure high-quality data, we perform:
- Handling missing values (imputation & dropping critical NaNs)
- Feature engineering (BMI & Avg BPM calculations)
- Encoding categorical variables (One-Hot Encoding)
- Scaling numerical features using **StandardScaler**

## 💪 Model Architecture

We use a **Deep Neural Network** with the following structure:
- **Dense(128, ReLU) + Dropout(0.3)**
- **Dense(128, ReLU) + Dropout(0.3)**
- **Dense(64, ReLU)**
- **Dense(1) (Output Layer)**
- **Optimizer:** Adam
- **Loss Function:** Mean Squared Error (MSE)

## 📈 Training & Evaluation

The model is trained using **early stopping** for optimal performance. We evaluate using:
- **Training & Validation Loss**
- **Learning Curves Visualization**

## 🎨 Visualization

The learning curve is plotted to observe model performance over epochs:
```python
plt.plot(history.history['val_loss'], label='Validation Loss')
plt.plot(history.history['loss'], label='Training Loss')
plt.xlabel('Epochs')
plt.ylabel('Loss')
plt.legend()
plt.show()
```

## 🎉 Enjoy exploring fitness insights and predictions! 

Happy coding! 🚀

