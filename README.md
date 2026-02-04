# 🚕 Taxi Demand Forecasting Using LSTM and PyTorch

## Project Overview
This project focuses on predicting future taxi demand using historical time series data.  
The model learns patterns from past taxi usage and forecasts upcoming demand to support better planning and decision making.

An LSTM based neural network implemented using PyTorch is used to capture temporal dependencies in taxi demand data.

---

## Problem Statement
Taxi service providers often struggle to balance supply and demand.

- Low demand prediction causes idle drivers  
- High demand underestimation causes long customer waiting times  

This project aims to build a time series forecasting model that predicts future taxi demand based on historical data.

---

## Dataset Description
The dataset contains time based taxi demand records collected at regular intervals.

### Columns
- **timestamp**. Date and time of observation  
- **value**. Number of taxi trips or taxi demand at that time  

This dataset represents time series data and is suitable for forecasting problems.

---

## Project Approach

### 1. Data Preprocessing
- Removed unnecessary index column  
- Converted timestamp to datetime format  
- Sorted data based on time order  

### 2. Exploratory Data Analysis
- Visualized taxi demand over time  
- Observed demand patterns such as peak and low hours  

### 3. Data Normalization
- Applied Min Max scaling to taxi demand values  
- Improved neural network training stability  

### 4. Sequence Creation
- Converted time series data into input output sequences  
- Used past demand values to predict future demand  

### 5. Model Building
- Built an LSTM based neural network using PyTorch  
- Used the last hidden state for prediction  

### 6. Model Training
- Trained the model using Mean Squared Error loss  
- Optimized using Adam optimizer  

### 7. Model Evaluation
- Compared predicted demand with actual demand  
- Visualized prediction results  

---

## Model Architecture
The model consists of the following components:

- Input. Past taxi demand values  
- LSTM layer. Learns temporal demand patterns  
- Fully connected layer. Predicts future taxi demand  

The model outputs the predicted demand for the next time step.

---

## Output
The model predicts future taxi demand values based on historical data.

### Example Outputs
- Taxi demand for next 30 minutes  
- Actual vs predicted taxi demand graph  

---

## Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- PyTorch  
- Scikit Learn  

---

## How to Run the Project

###  Install Dependencies
```bash
pip install pandas numpy matplotlib torch scikit-learn
