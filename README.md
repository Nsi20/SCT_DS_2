# Titanic Dataset Analysis: Data Cleaning and Exploratory Data Analysis (EDA)

This repository contains the implementation of **Task 2** from my ongoing project at **SkillCraft Technology**, where I performed **data cleaning**, conducted **Exploratory Data Analysis (EDA)**, and explored relationships between variables to identify key patterns and trends in the Titanic dataset.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Objectives](#objectives)
4. [Steps Taken](#steps-taken)
   - [1. Data Cleaning](#1-data-cleaning)
   - [2. Exploratory Data Analysis (EDA)](#2-exploratory-data-analysis-eda)
5. [Key Findings](#key-findings)
6. [Technologies Used](#technologies-used)
7. [How to Use](#how-to-use)
8. [Acknowledgments](#acknowledgments)

---

## Introduction
The Titanic dataset is one of the most well-known datasets in data science and is often used for learning and practising data analysis techniques. This project focuses on cleaning the data, uncovering patterns, and analyzing survival rates based on various factors such as gender, age, family size, and class.

---

## Dataset Description
The Titanic dataset consists of information on 891 passengers, including:
- **PassengerId**: Unique identifier for each passenger.
- **Survived**: Survival status (1 = Survived, 0 = Did not survive).
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd).
- **Name**: Name of the passenger.
- **Sex**: Gender of the passenger.
- **Age**: Age of the passenger.
- **SibSp**: Number of siblings/spouses aboard.
- **Parch**: Number of parents/children aboard.
- **Ticket**: Ticket number.
- **Fare**: Ticket price.
- **Cabin**: Cabin number.
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

---

## Objectives
1. Clean the dataset by handling missing values, formatting columns, and ensuring data quality.
2. Perform Exploratory Data Analysis (EDA) to explore relationships between features.
3. Identify trends and patterns influencing survival outcomes.

---

## Steps Taken

### 1. Data Cleaning
- **Missing Values**:
  - Imputed missing values in the `Age` column with the median age.
  - Filled missing values in the `Embarked` column with the mode (most frequent value).
  - Dropped the `Cabin` column due to excessive missing values (77% of entries).
- **Feature Engineering**:
  - Created a new feature `FamilySize` as the sum of `SibSp` and `Parch` to analyze the impact of travelling with family on survival.
  - Grouped the `Age` column into age categories: *Child*, *Teenager*, *Young Adult*, *Adult*, and *Senior* for better visualization.
- **Data Validation**:
  - Ensured no missing values remained in the dataset after cleaning.

### 2. Exploratory Data Analysis (EDA)
#### Visualizations
1. **Survival Rate by Gender**:
   - A bar chart showcasing the significantly higher survival rate of females compared to males.
2. **Survival Rate by Age Group**:
   - Analysis revealed that children had the highest survival rate among all age groups.
3. **Impact of Passenger Class (Pclass)**:
   - First-class passengers had a higher chance of survival compared to those in second and third classes.
4. **Effect of Family Size on Survival**:
   - Passengers travelling with small families (1-3 members) had slightly better survival rates than solo travellers or those with large families.

---

## Key Findings
1. **Gender**: Females had a significantly higher survival rate than males, likely due to prioritization during evacuation.
2. **Class**: Passengers in higher classes (1st class) had a better chance of survival compared to lower classes.
3. **Age**: Children had the highest survival rates, highlighting "women and children first" evacuation protocols.
4. **Family Size**: Traveling with family provided a slight advantage, but very large families faced lower survival rates.
5. **Embarked**: Passengers who boarded from Cherbourg (C) had better survival rates compared to other embarkation points.

---

## Technologies Used
- **Python**: Data manipulation and analysis.
- **Pandas**: For data cleaning and preprocessing.
- **NumPy**: Numerical computations.
- **Matplotlib & Seaborn**: Data visualization.

---

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/Nsi20/SCT_DS_2.git
   ```
2. Open the notebook in Jupyter or Google Colab.
3. Install the necessary dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
4. Run the notebook to see the analysis.

---

## Acknowledgments
Special thanks to **SkillCrafe** for this insightful project and to the Kaggle community for providing the Titanic dataset.

---
