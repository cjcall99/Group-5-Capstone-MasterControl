[Group 5: MSBA Capstone – MasterControl Lead Progression Analytics](https://github.com/amiyaranjan20-lgtm/MSBA_Capstone_Mastercontrol)

# Introduction

Why does MasterControl’s **Mx product line convert leads at a lower rate than its Qx product**, and how can data help improve this performance?

This repository contains the analytical work completed as part of the **MSBA Capstone Project at the University of Utah**, in collaboration with MasterControl. The project focuses on analyzing qualified account leads and building predictive models to identify which companies are most likely to progress through the sales pipeline for the **Mx manufacturing software solution**.

Through exploratory data analysis and predictive modeling, the project aims to uncover patterns in **industries, company characteristics, and buyer roles** that influence lead progression. The goal is to generate **data-driven recommendations that can help improve outbound targeting strategies and increase conversion rates for the Mx product line.**

---

# 1. Business Context and Objective

MasterControl provides enterprise software solutions to **life sciences organizations**, primarily through two product families:

- **Qx** – Quality management solutions  
- **Mx** – Manufacturing operations solutions  

While the **Qx product has achieved strong market adoption with progression rates near 19.7%**, the **Mx product currently progresses at approximately 12.7%**, indicating a notable performance gap between the two offerings.

This difference suggests that the current sales and marketing strategy for Mx may not be effectively identifying and targeting the organizations most likely to adopt manufacturing-focused software solutions.

At present, MasterControl lacks clear visibility into:

- Which **industries and manufacturing models** represent the strongest fit for the Mx solution  
- Which **company sizes and operational characteristics** correlate with higher conversion rates  
- Which **job roles and buyer personas** are most likely to influence purchasing decisions for manufacturing software  

As a result, outreach efforts may be spread across many organizations that are not ideal candidates for the product.

The guiding business question for this project is:

> Which companies and buyer roles are most likely to progress through the sales pipeline for the Mx product?

The core objectives of this analysis are to:

- Identify **high-propensity customer segments** for the Mx product  
- Understand differences between **Qx and Mx buyer profiles**  
- Develop **predictive models** that estimate the likelihood of lead progression  
- Provide **data-driven targeting recommendations** that can improve conversion rates and sales productivity  

---

# 2. Analytics Workflow Overview

The analysis follows a structured and reproducible analytics workflow consisting of several stages:

1. Data understanding and preparation  
2. Exploratory data analysis  
3. Feature engineering and preprocessing  
4. Predictive modeling and model comparison  
5. Interpretation of model results for business insights  

---

## 2.1 Data Understanding and Initial Cleaning

The first step involved reviewing the dataset structure and ensuring the data was suitable for analysis.

Key steps included:

- Examining dataset dimensions, variable types, and attribute descriptions  
- Standardizing variable names and formats  
- Identifying missing values and inconsistent entries  
- Cleaning categorical fields such as **industry, job title, and company type**  
- Preparing the dataset for exploratory and predictive analysis  

These steps ensured that the dataset was consistent, interpretable, and ready for further analysis.

---

## 2.2 Exploratory Data Analysis (EDA)

Before building predictive models, an exploratory analysis was conducted to better understand the structure and behavior of the data.

The EDA process focused on identifying patterns related to lead progression, including:

- Distribution of leads across **Qx and Mx products**
- Differences in **conversion rates between product lines**
- Relationships between **industries, company sizes, and progression outcomes**
- Patterns across **job titles, functional roles, and seniority levels**
- Identification of variables that show early signals of progression likelihood

This exploratory stage helped reveal important trends in the dataset and informed the feature selection and modeling strategy.

The full exploratory analysis is documented in:

`Group-5 EDA-MasterControl.Rmd`

---

## 2.3 Data Preparation and Feature Engineering

To prepare the dataset for predictive modeling, several preprocessing and feature engineering steps were applied.

These steps included:

- Handling missing values across account and contact attributes  
- Encoding categorical variables such as industry and job titles  
- Creating derived variables that capture company characteristics and buyer roles  
- Structuring the dataset to ensure compatibility with machine learning algorithms  

These preprocessing steps ensured consistent inputs across all models evaluated during the project.

---

## 2.4 Train and Validation Split

To evaluate model performance reliably:

- The dataset was divided into **training and validation subsets**  
- Models were trained using the training dataset  
- Model performance was evaluated using unseen validation data  

This approach helps ensure that model results **generalize well and are not driven by overfitting to the training data.**

---

## 2.5 Model Development

Several supervised learning algorithms were evaluated to predict whether a lead would **progress to the next stage in the sales pipeline**.

The models considered in the analysis include:

1. Logistic Regression  
2. Decision Tree (CART)  
3. Random Forest  
4. Gradient Boosting (XGBoost)

Each model was trained using a consistent dataset and preprocessing workflow to allow meaningful comparison across modeling approaches.

The full modeling workflow is documented in:

`Modeling_Mastercontrol_Group_5.Rmd`

---

## 2.6 Model Performance and Model Selection

Multiple modeling approaches were evaluated to identify a method that both predicts lead progression effectively and supports meaningful business interpretation.

The models assessed during this phase included:

- Logistic Regression  
- Decision Tree (CART)  
- Random Forest  
- Gradient Boosting (XGBoost)

Tree-based ensemble models demonstrated strong ability to capture **non-linear relationships and interactions between company characteristics, industries, and buyer roles**. These models provided valuable predictive insights into patterns within the dataset.

However, the objective of this project was not only predictive performance but also **clear interpretability that could support business decision-making.**

For this reason, **Logistic Regression was selected as the primary model for interpreting results and generating recommendations.**

Logistic regression provides several advantages that align well with the goals of the analysis:

- **Statistical significance testing (p-values)** helps identify which variables meaningfully influence lead progression  
- **Odds ratios** provide interpretable measures of how specific attributes increase or decrease progression likelihood  
- The model framework allows insights to be translated directly into **actionable guidance for sales and marketing teams**

In practical analytics work, the most complex algorithm is not always the most useful.

Often, **a simpler and interpretable model can generate clearer insights and stronger business value than more complex methods.**

Using logistic regression allowed the team to answer key business questions such as:

- Which industries show higher progression likelihood?  
- Which company characteristics influence lead success?  
- Which buyer roles are most likely to move forward in the sales pipeline?

This approach ensured that the results remained both **statistically sound and easily interpretable for business stakeholders.**

---

# 3. Project Contributions

This repository documents the analytical work conducted by the project team, including:

- Data exploration and dataset understanding  
- Exploratory data analysis to identify lead progression patterns  
- Data preparation and preprocessing for modeling  
- Development and comparison of predictive models  
- Interpretation of results from a business perspective  
- Documentation of insights and recommendations

The repository provides a complete record of the analytical process used to address the MasterControl business problem.

---

# 4. Business Value of the Analysis

The findings from this project provide several insights that can help improve MasterControl’s outbound targeting strategy.

Specifically, the analysis can help the organization:

- Identify **high-probability accounts for the Mx product**
- Improve **lead conversion rates**
- Focus sales outreach on organizations with the strongest product fit
- Increase **sales development representative (SDR) productivity**
- Strengthen alignment between marketing campaigns and ideal customer profiles

By prioritizing high-propensity segments, MasterControl can allocate resources more effectively and improve adoption of the Mx product.

---

# 5. Challenges Encountered

Several analytical challenges influenced the project:

1. High variability in **job titles and buyer roles**
2. Complex categorical variables such as **industry classifications**
3. Missing or incomplete information across some account attributes
4. Differences between buyer personas associated with **Qx and Mx products**

Addressing these challenges required careful preprocessing, feature engineering, and thoughtful model selection.

---

# 6. What We Learned

This project strengthened several applied analytics and data science skills, including:

- Translating business questions into analytical frameworks  
- Conducting structured exploratory data analysis  
- Preparing real-world datasets for machine learning models  
- Comparing multiple modeling approaches  
- Communicating analytical findings in clear business language  

The project represents a full **end-to-end analytics workflow similar to real industry consulting engagements.**

---

# 7. Interpretation of Results and Key Takeaways

The analysis revealed several important insights about lead progression for the Mx product.

### Key Findings

**1. Product positioning influences conversion**

The Mx product currently converts leads at a lower rate than Qx, suggesting opportunities to refine targeting strategies.

**2. Industry and manufacturing characteristics matter**

Organizations with stronger manufacturing operations appear more aligned with the Mx product offering.

**3. Buyer personas differ between product lines**

Decision-makers responsible for manufacturing operations may differ significantly from those responsible for quality management systems.

**4. Predictive analytics improves targeting**

Machine learning models help identify patterns in company attributes and buyer roles that correlate with higher progression likelihood.

These findings support the development of a **data-driven outbound strategy** for MasterControl’s sales and marketing teams.

---

# 8. Repository Contents

- `Business Problem Statement(Group 5).pdf`  
  Overview of the business problem, project scope, and success metrics.

- `Group 5 Presentation.pptx.pdf`  
  Final presentation summarizing the analytical approach, modeling results, and key business insights.

- `Group-5 EDA-MasterControl.Rmd`  
  R Markdown notebook containing the full exploratory data analysis.

- `Modeling_Mastercontrol_Group_5.Rmd`  
  R Markdown file documenting the predictive modeling workflow and model evaluation.

- `README.md`  
  Project documentation describing the analytical approach, results, and repository structure.
