# Tourism Revenue Prediction Project

This project focuses on analyzing tourism-related data and building machine learning models to predict tourism revenue. 
The project applies data preprocessing, exploratory data analysis (EDA), feature engineering, and predictive modeling techniques to identify important factors affecting revenue performance.

The workflow was developed using Python and Jupyter Notebook as part of a data analytics and machine learning practice project.

---

## Objectives

The main objectives of this project are:

- Analyze tourism-related datasets
- Explore relationships between attendance and revenue
- Perform data cleaning and preprocessing
- Apply feature engineering techniques
- Build predictive machine learning models
- Evaluate model performance using regression metrics

---

## Team Members & Responsibilities

The project was carried out by Group 5, with each member contributing to specific aspects of the project as follows:

| Name | Student ID | Role | Responsibilities |
|------|------|------|------|
| Tran Hoang Anh | 11247449 | Team Leader / Data Analyst | Participated in all three stages of the project, including data cleaning, exploratory data analysis (EDA), preprocessing, machine learning modeling, and project content integration. |
| Nguyen Thi Diu | 123458 | Data Analyst | Supported data cleaning in `01_LamSachDuLieu.ipynb`, exploratory data analysis (EDA), and data visualization. |
| Do Anh Duong | 11247455 | Data Engineer / ML Support | Analyzed key characteristics of the dataset in `02_KhamPhaDuLieu.ipynb`, while also supporting model interpretation and feature importance analysis in the modeling stage. |
| Le Hieu Minh | 11247481 | Machine Learning Engineer | Supported preprocessing, model building, and model training in `03_HuanLuyenModel.ipynb`, evaluated model performance, and completed the `README.md` file. |

In addition to their main responsibilities, all team members contributed to dataset searching, research ideation, and discussions regarding the project direction and implementation.
---

## Repository Structure

```bash
project/
│
├── data/
│   ├── raw_data.csv
│   └── cleaned_data.csv
│
├── notebooks/
│   ├── 01_KhamPhaDuLieu.ipynb
│   ├── 02_LamSachDuLieu.ipynb
│   └── 03_HuanLuyenModel.ipynb
│
├── images/
│
├── models/
│
├── README.md
│
└── requirements.txt
```

---

## Dataset

### Data Source
- Kaggle Dataset: Taylor Concert Tours Impact on Attendance and Revenue

### Description
The dataset contains 445 rows and 8 columns related to concert tours between 2009 and 2018.  
It includes information such as city, country, venue, opening acts, tickets sold, total available tickets, attendance rate, and concert revenue.

---

## Main Variables

- `Revenue`
- `Tickets_Sold`
- `Attendance_Rate`
- `Attendance_Level`
- `Tour`
- `Ticket_Price`

---

## Data Preprocessing

Several preprocessing techniques were applied during the project.

### Steps Included

### 1. Handling Missing Values
- Identified missing values
- Removed or transformed problematic records

### 2. Outlier Detection
- Checked abnormal values
- Reduced noise in the dataset

### 3. Encoding
- Converted categorical variables into numerical formats

### 4. Feature Engineering
- Created attendance categories
- Performed variable binning

### 5. Data Transformation
- Standardized numerical variables when necessary

---

## Exploratory Data Analysis (EDA)

EDA was conducted to understand the dataset and discover important insights.

### Analysis Performed

- Distribution analysis
- Correlation analysis
- Revenue trend analysis
- Outlier visualization
- Relationship between attendance and revenue

### Visualization Libraries

- Matplotlib
- Seaborn

---

## Machine Learning Models

The project used regression models to predict concert revenue.

### Models Applied

### Linear Regression
Used as the baseline model for prediction.

### Random Forest Regressor
Used to improve prediction performance and capture non-linear relationships.

---

## Evaluation Metrics

The models were evaluated using:

- RMSE (Root Mean Squared Error)
- Mean Squared Error (MSE)
- R² Score

These metrics help measure prediction accuracy and model reliability.

---

## Key Findings

### Regarding Data

Through exploratory data analysis (EDA), the team found that revenue is strongly right-skewed (`skewness = 2.32`), largely driven by Reputation Stadium Tour shows — reflecting a significant gap in production scale across tours.

`Tickets_Sold` showed the strongest correlation with revenue (`r = 0.96`), while geographic distribution was heavily concentrated in Foxborough, Philadelphia, and East Rutherford — the top three highest-revenue cities across all tours.

### Regarding Models

The project applied two complementary modeling approaches:

#### Predictive Modeling
Random Forest outperformed Linear Regression with:

- `R² = 0.953` for Random Forest
- `R² = 0.832` for Linear Regression

This confirms the presence of nonlinear relationships in concert revenue data, with ticket sales being the strongest predictor.

#### Explanatory Modeling
After removing ticket-related variables, `Tour` identity emerged as the most important structural factor (`R² = 0.621`), suggesting that tour branding and artist popularity play a decisive role in revenue differences across concerts.

### Main Insights

- Attendance rate strongly impacts concert revenue
- Feature engineering improved model performance
- Random Forest performed better than Linear Regression
- Data preprocessing significantly improved prediction quality

---

## Technologies Used

### Programming Language
- Python

### Libraries
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- pathlib

### Development Environment
- Jupyter Notebook
- VS Code

---

## Installation

Install required libraries using:

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Step 1: Open Jupyter Notebook

```bash
jupyter notebook
```

### Step 2: Run notebooks in order

1. `01_KhamPhaDuLieu.ipynb`
2. `02_LamSachDuLieu.ipynb`
3. `03_HuanLuyenModel.ipynb`

---

## Future Improvements

Possible future improvements include:

- Hyperparameter tuning
- Testing additional machine learning models
- Deploying the model as a web application
- Improving feature engineering techniques
- Expanding the dataset

---

## Conclusion

This project demonstrates a complete machine learning workflow for concert revenue prediction, including data preprocessing, exploratory analysis, feature engineering, model training, and evaluation.

The findings highlight the importance of attendance behavior, ticket sales, and tour branding in predicting concert revenue performance.

---

## Academic Context

*This project was developed for academic purposes in the field of Data Science for Economics and Business at National Economics University (NEU), 2026.*