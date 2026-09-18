#  Unemployment Dashboard in Nigeria

##  Project Overview

The **Unemployment Dashboard in Nigeria** is a data analytics and visualization project developed to explore unemployment patterns across different demographic and socioeconomic groups in Nigeria.

The project uses data cleaning, exploratory data analysis (EDA), and interactive visualization to examine unemployment records by **age, gender, education level, employment status, and region**.

---

## Objective

The objective of this project is to analyze unemployment patterns in Nigeria, with a primary focus on **age groups**, while examining how unemployment records vary by gender, education level, employment status, and region.

The analysis aims to provide data-driven insights that can improve understanding of the groups represented in unemployment records and support discussions around employment opportunities, skills development, and targeted workforce interventions.

---

## Data Source

The dataset was obtained from Kaggle:

**Nigeria Unemployment Dataset**

https://www.kaggle.com/datasets/awofiranyejames/nigeria-unemployment-dataset/data

---

## Dataset Description

The original dataset contains **5,000 records** and includes information on:

- Age
- Gender
- Region
- Location
- Education Level
- Employment Status
- Years of Experience
- Monthly Income (NGN)

After removing **25 duplicate records**, **4,975 unique records** were used for analysis.

The employment status categories are:

- Employed
- Unemployed
- Underemployed

---

##  Data Cleaning and Preparation

The following data preparation steps were carried out:

- Checked the dataset for missing values and duplicates.
- Removed **25 duplicate records**.
- Replaced missing values in **Region, Education Level, and Years of Experience** with `N/A` where appropriate.
- Retained missing **Monthly Income** values rather than treating them as zero.
- Created an **Age Group** variable using the following categories:
  - 15–24
  - 25–34
  - 35–44
  - 45–54
  - 55–64
- Created an **Unemployment Flag** to identify records classified as unemployed.

The cleaned dataset was then imported into **Power BI** for analysis and visualization.

---

##  Exploratory Data Analysis (EDA)

Exploratory analysis was conducted to understand the distribution of employment and unemployment records across key demographic and socioeconomic variables.

The analysis focused on:

- Overall employment status distribution
- Unemployment records by age group
- Unemployment records by gender
- Unemployment records by education level
- Regional distribution of unemployment records

The analysis also distinguished between **unemployment counts** and **group-specific unemployment rates** where the available data allowed the comparison.

---

# Key Findings

## 1. Overall Employment Status

Out of **4,975 records**:

| Employment Status | Records | Share |
|---|---:|---:|
| Underemployed | 2,206 | 44.3% |
| Employed | 1,816 | 36.5% |
| Unemployed | 953 | 19.2% |

Underemployed records represented the largest share of the dataset, while unemployed records accounted for approximately **19.2%**.

This highlights that underemployment represents a substantial component of the employment situation captured in the dataset.

---

## 2. Unemployment by Age Group

The number of unemployed records across the five age groups was relatively evenly distributed:

| Age Group | Unemployed Records |
|---|---:|
| 45–54 | 198 |
| 15–24 | 195 |
| 35–44 | 194 |
| 55–64 | 188 |
| 25–34 | 178 |

The **45–54 age group** recorded the highest number of unemployed records, while the **25–34 age group** recorded the lowest.

However, when unemployment was considered relative to the size of each age group, the **15–24 age group recorded the highest unemployment share at approximately 20.2%**.

The relatively small differences between age groups suggest that unemployment in this dataset is not overwhelmingly concentrated in a single age category.

---

## 3. Unemployment by Gender

Unemployment was almost evenly distributed between males and females.

| Gender | Unemployed Records | Share |
|---|---:|---:|
| Male | 483 | 50.7% |
| Female | 470 | 49.3% |

The difference between male and female unemployment representation was relatively small, indicating a near-even gender distribution among unemployed records in the dataset.

---

## 4. Unemployment by Education Level

The **secondary education** group recorded the highest number of unemployed records, with **341 records**.

However, when unemployment was considered relative to the size of each education group, the **tertiary-educated group recorded the highest unemployment rate at approximately 36.8%**.

This demonstrates that unemployment in the dataset is not limited to individuals with lower educational attainment and highlights the importance of examining graduate employment and the transition from education into the labour market.

---

## 5. Regional Distribution

The **North West** recorded the highest number of unemployed records, with **215 records**, representing approximately **22.6% of all unemployed records**.

The **South East** recorded the lowest number of unemployed records, with **96 records**.

However, when the size of each regional group was considered, the **North East recorded the highest unemployment rate at approximately 21.0%**.

This demonstrates the importance of examining both **unemployment counts and group-specific rates** when comparing regions.

---

# Dashboard

The interactive Power BI dashboard allows users to explore unemployment patterns across different demographic and geographic categories.

### Dashboard Features

- Employment Status Distribution
- Unemployment Records by Age Group
- Unemployment Records by Gender
- Unemployment Records by Education Level
- Unemployment Records by Region
- Region slicer
- Age Group slicer
- KPI cards for employment status

### Dashboard Preview

![Nigeria Unemployment Dashboard](https://drive.google.com/file/d/1oSzfBwKswy7v68XK18BJdQ_dsOTcVTvZ/view?usp=drivesdk)

---

# Recommendations

### 1. Develop Employment Interventions Across Age Groups

Since unemployment records were relatively evenly distributed across age categories, employment initiatives should not focus exclusively on young people.

### 2. Strengthen Graduate Employability Programmes

The relatively high unemployment rate among tertiary-educated individuals highlights the need for practical skills development, internships, career-transition programmes, and stronger connections between education and industry.

### 3. Promote Market-Relevant Skills Development

Vocational, digital, technical, and professional skills programmes can complement formal education and help improve alignment between workforce skills and labour-market opportunities.

### 4. Adopt Region-Specific Employment Strategies

Regional differences in unemployment suggest that employment interventions should consider local economic conditions, labour-market opportunities, and skills requirements.

---

#  Tools Used

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Data cleaning and preparation |
| **Power BI** | Data analysis, visualization, and dashboard development |
| **DAX** | Measures and calculated fields |
| **GitHub** | Project documentation and portfolio presentation |

---

#  Project Structure

```text
Nigeria-Unemployment-Dashboard/
│
├── README.md
│
├── data/
│   └── cleaned_nigeria_unemployment.xlsx
│
├── dashboard/
│   └── Nigeria_Unemployment_Dashboard.pbix
│
└── images/
    └── dashboard.png
