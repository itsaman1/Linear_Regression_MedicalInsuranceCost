# Medical Charges Prediction using Linear Regression

## 📌 Overview
This project applies **Linear Regression** to predict **medical insurance charges** based on a patient’s characteristics such as **age, BMI, smoking habits, and region**. By analyzing these features, the model estimates medical expenses, helping insurers and healthcare providers understand cost patterns.


Every machine learning problem has three components:

1. **Model**

2. **Cost Function**

3. **Optimizer**

We'll look at several examples of each of the above in future tutorials. Here's how the relationship between these three components can be visualized:

<img src="https://i.imgur.com/oiGQFJ9.png" width="480">

## 📊 Dataset
- The dataset consists of **1,338 records** with the following columns:
  - `age` - Age of the individual
  - `sex` - Gender (Male/Female)
  - `bmi` - Body Mass Index (BMI)
  - `children` - Number of dependents
  - `smoker` - Whether the person is a smoker or not
  - `region` - Residential region
  - `charges` - Medical insurance cost (Target variable)

## 🔍 Key Features
- **Exploratory Data Analysis (EDA):**
  - Data cleaning and handling missing values
  - Correlation analysis to identify key influencing factors
  
- **Feature Engineering & Model Training:**
  - Encoding categorical variables using **one-hot encoding**
  - Splitting dataset into **training (80%)** and **testing (20%)**
  - Implementing **Linear Regression** using `scikit-learn`
  
- **Model Evaluation:**
  - Performance measured using **R² score, MAE, and RMSE**
  - Observed that **smoking habits significantly increase medical charges**
  - Feature scaling and optimization techniques explored

## 🛠 Technologies Used
- **Python** 🐍
- **Pandas & NumPy** (Data Processing)
- **Scikit-learn** (Machine Learning)
- **Matplotlib & Seaborn** (Data Visualization)

## 🚀 Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/Medical-Charges-Prediction.git
   cd Medical-Charges-Prediction
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook LinearRegression1.ipynb
   ```

## 📈 Insights & Learnings
- **Smoking is the most influential factor in determining medical charges** 📊
- **Age and BMI have a strong correlation with medical expenses**
- **Linear Regression performs well for this dataset, but feature engineering can further improve predictions**

## 🤝 Contributions
Feel free to fork the repository, raise issues, or submit pull requests! 🚀

📢 **Let’s connect!** If you have suggestions or insights, I’d love to discuss them. 😊

---

🔗 **GitHub Repository:** [Insert Repo Link]

