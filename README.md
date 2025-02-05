# Medical Charges Prediction using Linear Regression

## 📌 Overview
This project applies **Linear Regression** to predict **medical insurance charges** based on a patient’s characteristics such as **age, BMI, smoking habits, and region**. By analyzing these features, the model estimates medical expenses, helping insurers and healthcare providers understand cost patterns.


Every machine learning problem has three components:

1. **Model**

2. **Cost Function**

3. **Optimizer**

The relationship between these three components can be visualized:

<img src="https://i.imgur.com/oiGQFJ9.png" width="480">

Here's how correlation coefficients can be interpreted ([source](https://statisticsbyjim.com/basics/correlations)):

* **Strength**: The greater the absolute value of the correlation coefficient, the stronger the relationship.

    * The extreme values of -1 and 1 indicate a perfectly linear relationship where a change in one variable is accompanied by a perfectly consistent change in the other. For these relationships, all of the data points fall on a line. In practice, you won’t see either type of perfect relationship.

    * A coefficient of zero represents no linear relationship. As one variable increases, there is no tendency in the other variable to either increase or decrease.
    
    * When the value is in-between 0 and +1/-1, there is a relationship, but the points don’t all fall on a line. As r approaches -1 or 1, the strength of the relationship increases and the data points tend to fall closer to a line.


* **Direction**: The sign of the correlation coefficient represents the direction of the relationship.

    * Positive coefficients indicate that when the value of one variable increases, the value of the other variable also tends to increase. Positive relationships produce an upward slope on a scatterplot.
    
    * Negative coefficients represent cases when the value of one variable increases, the value of the other variable tends to decrease. Negative relationships produce a downward slope.

Here's the same relationship expressed visually ([source](https://www.cuemath.com/data/how-to-calculate-correlation-coefficient/)):

<img src="https://i.imgur.com/3XUpDlw.png" width="360">

The correlation coefficient has the following formula:

<img src="https://i.imgur.com/unapugP.png" width="360">

You can learn more about the mathematical definition and geometric interpretation of correlation here: https://www.youtube.com/watch?v=xZ_z8KWkhXE

### Optimizer

Next, we need a strategy to modify weights `w` and `b` to reduce the loss and improve the "fit" of the line to the data.

* Ordinary Least Squares: https://www.youtube.com/watch?v=szXbuO3bVRk (better for smaller datasets)
* Stochastic gradient descent: https://www.youtube.com/watch?v=sDv4f4s2SB8 (better for larger datasets)

Both of these have the same objective: to minimize the loss, however, while ordinary least squares directly computes the best values for `w` and `b` using matrix operations, while gradient descent uses a iterative approach, starting with a random values of `w` and `b` and slowly improving them using derivatives. 

Here's a visualization of how gradient descent works:

![](https://miro.medium.com/max/1728/1*NO-YvpHHadk5lLxtg4Gfrw.gif)

Doesn't it look similar to our own strategy of gradually moving the line closer to the points?

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

