# Titanic Survivors Analysis

This repository contains an in-depth analysis of the Titanic survivors using a Jupyter Notebook. The goal of this project is to explore, analyze, and predict the factors that influenced the survival of passengers aboard the Titanic.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Analysis](#analysis)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The Titanic Survivors Analysis project aims to explore the Titanic dataset, identifying key factors that affected passenger survival rates. This project involves data cleaning, exploratory data analysis, feature engineering, and applying machine learning algorithms to predict survival outcomes.

## Dataset

The dataset used in this project is the Titanic dataset, which is widely available and hosted on [Kaggle](https://www.kaggle.com/c/titanic/data). It includes information about the passengers, such as:

- Passenger ID
- Survival (0 = No, 1 = Yes)
- Pclass (Ticket class)
- Name
- Sex
- Age
- SibSp (Number of siblings/spouses aboard)
- Parch (Number of parents/children aboard)
- Ticket number
- Fare
- Cabin
- Embarked (Port of Embarkation: C = Cherbourg, Q = Queenstown, S = Southampton)

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/Titanic-Survivors-Analysis.git
    ```
2. **Navigate to the project directory:**
    ```bash
    cd Titanic-Survivors-Analysis
    ```
3. **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    Ensure you have Python and pip installed on your system. The `requirements.txt` file includes the following necessary packages:
    - `pandas`
    - `numpy`
    - `matplotlib`
    - `seaborn`
    - `scikit-learn`
    - `jupyter`

## Usage

To execute the analysis:

1. **Start Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
2. **Open the notebook:**
    In the Jupyter interface, open the `Titanic_Survivors.ipynb` file.
3. **Run the cells:**
    Execute the cells in the notebook to perform the data analysis, visualization, and model predictions.

## Analysis

The analysis covers the following steps:

1. **Data Cleaning:**
   - Handle missing data in columns like `Age`, `Cabin`, and `Embarked`.
   - Convert categorical variables like `Sex` and `Embarked` into numerical values.

2. **Exploratory Data Analysis (EDA):**
   - Visualize the distribution of passengers by class, gender, and survival status.
   - Analyze correlations between different features and the survival rate.
   - Identify any patterns or insights that might be useful for modeling.

3. **Feature Engineering:**
   - Create new features from the existing data, such as family size (combining `SibSp` and `Parch`) and title extraction from the `Name` column.
   - Normalize and scale features where necessary to improve model performance.

4. **Modeling:**
   - Train several machine learning models (e.g., DecisionTree, XGBoost, Random Forest, Support Vector Machine) to predict passenger survival.
   - Evaluate model performance using metrics like accuracy, precision, recall, and F1-score.
   - Tune model hyperparameters to improve predictions.

5. **Conclusion:**
   - Summarize the insights gained from the data analysis.
   - Discuss the model's performance and any limitations encountered.

## Results

The key findings of the analysis include:

- **Gender:** Female passengers had a significantly higher survival rate compared to males.
- **Class:** Passengers in the first class had a higher likelihood of survival compared to those in the third class.
- **Family Size:** Passengers with a small family size (1-3 members) had better survival chances than those traveling alone or with large families.
- **Fare:** Higher ticket fares were associated with higher survival rates, likely reflecting the class distribution.

The best-performing model achieved a recall of `74%`, demonstrating the effectiveness of the features selected and the model chosen.

## Contributing

Contributions to this project are welcome. If you have any ideas, suggestions, or find any issues, please feel free to fork the repository, create a branch, and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This README should be placed in your GitHub repository as `README.md`. It contains detailed information about the project, making it easy for others to understand, use, and contribute to your work.
