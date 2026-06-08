# Health Insurance Claims
Health Insurance Underwriting with Simulated Health Insurance Dataset

[Notebook Link](https://github.com/Sodiq-Shodimu/nexygen-project/blob/main/health-insurance-claims.ipynb)  

---

## Table of Contents

- [Overview](#overview)  
- [Dataset](#dataset)  
- [Technologies Used](#technologies-used)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Analysis & Visualizations](#analysis--visualizations)  
- [Conclusion](#conclusion)  
- [Credits](#credits)  
- [License](#license)  

---

## Overview

- The dataset was chosen to assess heath insurance uderwriting. 
-The objecive was to determine segmentation, risk scoring, data insights and  scenario testing

---

## Dataset
- The dataset is Medical Cost Personal Datasets from Kaggle
- Size of the dataset is 1338 rows and 7 columns  

---

<h2>Technologies Used</h2>

<ul>
  <li><strong>Languages & Libraries:</strong> Python, Pandas, NumPy, Matplotlib, Seaborn, sklearn</li>
  <li><strong>Tools:</strong> Jupyter Notebook, VS Code, Git, GitHub</li>
 
</ul>

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib">
  <img src="https://img.shields.io/badge/-Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Seaborn">
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="scikit-learn">
</p>

<P>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter Notebook"/>
  <img src="https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VS Code"/>  
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</p>
<p>
  <img src="https://img.shields.io/badge/MIT%20License-000000?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="MIT License">
</p>

---

## Installation

Step-by-step instructions to set up the project locally:

```bash

# Clone the repository
git clone git clone https://github.com/Kurodataio/Health-Insurance-Claims.git

# Navigate to the project folder
cd Health-Insurance-Claims

# Launch Jupyter Notebook
jupyter notebook


```

## Usage

Instructions for using the project:

1. Open the main notebook (`health-insurance-claims.ipynb`)  
2. Run ALL cells or each cell sequentially to reproduce the analysis  
3. Visualizations and results will be generated automatically  

---

## Analysis & Visualizations 

- **Age vs. Claims Cost (Smoker Highlighted)**
  - 3 clear bands with linear relationship between age and claims cost
  - Bottom blue non-smokers band has lowest age to claims cost
  - Middle non-smokers and smokers
  - Top orange smokers band has the gighest agr to claims cost
  - The is a clear positive linear relationship between age and claims cost
  - Smoking increases the cost of caims
- **BMI vs. Claims Cost**
  - For non-smokers BMI is minor impact on costs. Most claims costs for non smokers are below $15k
  - For smokers, there is significant BMI impact beyond BMI of 30
  - BMI minimal impact on claims costs for non-smokers however for BMI over 30 there is an sudden and increasing impact on costs
![Age_&_BMI_vs_Claims_Cost](images/Age_&_BMI_vs_Claims_Cost.png) 

- **Claims Cost by Smoker Status**
  - The average claims cost between smokers and non-smokers claims cost is significant
  - Non-smokers have a median cost of $7,500
  - Smokers have a mediam cost of $34,500
  - There is no overlap between the smoking and non-smoking groups
  - The 75th percentile for non-snokers is lower than the 25th percentile for smokers
  - For non smokers the claims cost are between $4,000 and $11,500
  - For smokers the claims cost are between $21,000 to $41,000
  - Smokers have a wider range (variance) of claims costs
  - Non smokers have many outlying claims around $23,000 up to $37,000
  - This plot shows high outliers for non-smokers are within the typical claims cost for smokers
![Claims_Cost_by_Smoker_Status](images/Claims_Cost_by_Smoker_Status.png)

- **Claims Cost by Dependents**
  - The average (median) claims cost for all groups is $8,000 and $11,000
  - 0 to 2 dependents: The median is around $8,500–$9,500
  - 3 to 4 dependents: The mdian peaks at $11,000 for 4 dependents
  - 5 dependents: The median is under $9,000
  - The group with 0 dependents has outliers with the highest cost of $60,000+
  - The group with 5 dependents has outliers with the lowest cost at under $20,000
  - The number of dependents does not dictate high claims cost. In fact it seems the opposite.
![Claims_Cost_by_Dependents](images/Claims_Cost_by_Dependents.png) 

- **Claims Cost by Gender**
  - Both genders have an average claim cost of $9,300.
  - Gender has no significance to median claim costs
  - Both genders have a long tail of outliers. Beyond $30K for Women and beyond $40k for men
![Claims_Cost_by_Gender](images/Claims_Cost_by_Gender.png) 

- **Claims Cost by Region**
  - Southwest, Southeast, Northwest have a median claims cost around $9k to $9.3k
  - Northeast has a higher median claims cost around $10k.
  - Region is a not a significant determinant of claims cost.
  - The Southeast has the highest range of claims costs. It also has the highest outlier costs
  - The outliers can be associated with risk factors such as smoking and high BMI
  - Does this suggest that the Southeast has more smokers and obese clients hence the higher claims costs
![Claims_Cost_by_Region](images/Claims_Cost_by_Region.png) 

- **Claims Cost Distribution by Smoking Status**
  - The non-smokers show right-skewed distribution
  - The highest frequency (density) of individuals show claims cost between $2,000 and $10,000.
  - The data shows that most of the minor claims are by non-smokers
  - The data shows two peaks for smokers. It is bimodal.
  - The first peak cluster is between $15,000–$25,000.
  - The second peak cluster is between $35,000–$50,000.
![Claims_Cost_Distribution_by_Smoking_Status.png](images/Claims_Cost_Distribution_by_Smoking_Status.png) 

- **Correlation_Heatmap**
  - The positive correlation between smoker and claims cost is 0.79
  - The positive correlation between age and claims cost is 0.30 and 0.20 for bmi and claims cost.
  - The heatmap does not show the interaction effect between BMI and smoking which is associated with higgher costs.
  - The heatmap clearly shows the following:
    - Smoker status (Highest correlation)
    - Age (High correlation)
    - BMI (Moderate correlation)
![Correlation_Heatmap](images/Correlation_Heatmap.png) 

- **Distribution of Claims Cost**
  - The distribution of claims is skewed to the right (positive) skewed
  - Most of the insurance claims are low to medium in costs
  - The distribution is bimodal, primary and secondary peaks
  - The two peaks suggest sub populations of claims cost
  - Mode about $2,000 to $3,000 - [calculate actual value]
  - Median about $8,000 to $10,000 - [calculate actual value]
  - Mean about $12,000 - $15,000 - [calculate actual value]
![Distribution_of_Claims_Cost](images/Distribution_of_Claims_Cost.png) 

-**Loss_Ratio_Distribution**
![Loss_Ratio_Distribution](images/Loss_Ratio_Distribution.png) 

- **Feature_Importance**
![Feature_Importance](images/Feature_Importance.png) 
<!-- ![title](images/image.png)  -->
<!-- ![title](images/image.png)  -->

---

## Conclusion 
- Summarize the outcome of your analysis  
- What are the main insights or takeaways?  
- How could this analysis inform decision-making?  
- Recommendations or next steps for further analysis  
- **Smoking and BMI combined are associated with the highest claims cost**
- **Are smoking and BMI signals for increased billing or actual indicators of assocated illness?**

---

## Credits

- **Dataset Source:** [Kaggle → Datasets](https://www.kaggle.com/datasets/mirichoi0218/insurance)  
- **Google Gemini** [Link](https://gemini.google.com/app)  
- **CoPilot** [Link](https://copilot.microsoft.com/)  

---

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/)

---
