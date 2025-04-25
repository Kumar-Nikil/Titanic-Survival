# Titanic Survival Prediction

## 🧠 Overview
This project analyzes the tragic 1912 sinking of the RMS Titanic through the lens of predictive modeling. By leveraging machine learning algorithms, the goal was to predict passenger survival based on key characteristics such as class, age, fare, and gender. The dataset was obtained from Kaggle, cleaned, transformed, and modeled using Python, with visual outputs presented through Tableau dashboards.

## ⚙️ Technologies & Tools
- **Languages & Libraries**: Python, Pandas, NumPy, Scikit-Learn, Matplotlib, TensorFlow, SQLite3
- **ML Models**: Neural Network, Logistic Regression, Random Forest
- **Visualization**: Tableau
- **Notebook/Platform**: Google Colab

## 🧹 Data Preparation
The dataset was preprocessed with the following steps:
- Filled missing values in `Age` and `Fare` with mean values
- One-hot encoded categorical columns (`Sex`, `Pclass`, `Embarked`)
- Dropped irrelevant columns: `Name`, `Ticket`, `Cabin`, `Boat`, `Body`, and `Index`
- Scaled features before modeling
- Target variable: `Survived` (0 = No, 1 = Yes)

## 🤖 Machine Learning Models

### 🔹 Neural Network
- Architecture: 2 hidden layers (24 and 12 neurons), ReLU activation; output layer with sigmoid
- Accuracy: ~83% on training, ~80% on testing
- Limitations: Minor performance improvement from tuning; dataset imbalance affected recall

### 🔹 Logistic Regression
- Straightforward model with clean, interpretable coefficients
- Accuracy: ~82% on testing — **best performing model overall**

### 🔹 Random Forest
- Ensemble model with decent performance
- Accuracy: ~80% on test set

## 📊 Visualization Dashboard
An interactive dashboard was created in Tableau to:
- Visualize survival distribution across passenger classes
- Analyze relationships between features and survival rate
- Enable drill-down insights into gender, age, and fare
- ![image](https://github.com/user-attachments/assets/f310cc13-04ea-4331-9414-ec32633f911c)


## 🔍 Insights & Observations
- All models performed well in accuracy and precision, but recall was weak for survivors due to class imbalance
- Logistic regression offered the best balance of interpretability and accuracy
- Further work could explore oversampling or using SMOTE for better recall performance

## 🚀 Future Work
- Build a **Streamlit web app** to let users input passenger data and predict survival in real time
- Use more advanced NLP techniques on name/title fields for richer feature extraction
- Integrate other public Titanic datasets to enhance feature diversity and model generalization

## 📁 Dataset Source
- [Titanic - Machine Learning from Disaster | Kaggle](https://www.kaggle.com/competitions/titanic/data)

---

👤 **Created by Nikil Kumar Karani Apparao Ramakrishnan**  
MS in Business Analytics | DePaul University  
[LinkedIn](http://www.linkedin.com/in/nikilkumarkr)
