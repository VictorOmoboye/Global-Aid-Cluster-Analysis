# GLOBAL AID CLUSTER ANALYSIS
## Leveraging Advanced Unsupervised Machine Learning for Data-Driven Clustering to Prioritize Aid for Vulnerable Nations
![image](https://github.com/user-attachments/assets/1781c069-8623-4e66-8a04-ea118cd5b361)

### INTRODUCTION
This project aims to support **HELP International**, a humanitarian NGO, in identifying and prioritizing countries most in need of aid by analyzing socio-economic and health metrics. Using advanced unsupervised machine learning techniques, the project clusters nations based on critical indicators like GDP per capita, child mortality, and life expectancy. By leveraging data-driven insights, it seeks to optimize resource allocation and address pressing global issues such as poverty, healthcare access, and welfare for vulnerable populations.
![image](https://github.com/user-attachments/assets/1adb2704-9a11-442c-888f-eaa356109424)

### PROBLEM STATEMENT
- HELP International seeks to identify countries facing critical socio-economic and health challenges, such as low GDP, high child mortality, and low life expectancy.
- The organization wants to prioritize resource allocation to nations most in need based on data-driven insights.
- A need exists to analyze large datasets containing socio-economic and health metrics to inform the distribution of aid effectively.
- The project must leverage machine learning clustering techniques to group countries by shared vulnerabilities.
- There is a requirement to explore patterns in the data that can guide actionable decisions to improve health, wealth, and opportunities in marginalized nations.

### AIM OF PROJECT
- To leverage advanced unsupervised machine learning techniques to cluster countries based on critical socio-economic and health metrics.
- To identify nations with low GDP, high child mortality, and low life expectancy that are most in need of aid.
- To provide data-driven insights that prioritize resource allocation for vulnerable populations.
- To optimize HELP International’s efforts in addressing global issues such as healthcare access, poverty, and gender equality.
- To ensure efficient and targeted distribution of the $30M donation by focusing on the most at-risk nations.

### METHODOLOGY

- **STEP 1:** Data Cleaning:
    - Handle any missing values.
    - Remove duplicate records or irrelevant columns.
    - Check for and correct anomalies.
      
- **STEP 2:** Exploratory Data Analysis (EDA):
    - Visualize distributions and relationships between features.
    - Identify patterns, trends, and potential anomalies.
    - Form hypotheses based on data insights.
      
- **STEP 3:** Data Preprocessing:
    - Scale/normalize numerical features and encode categorical  data.
    - Feature Engineering
      
- **STEP 4:** Model Training:
    - Select and train machine learning models on the data.
    - Elbow Method to find the optimal number of clusters (k).
    - Experiment with different algorithms and assess performance.
      
- **STEP 5:** Model Evaluation (Interpreting Results):
    - Visual Inspection: visualize the clustering results or reduced features to evaluate if meaningful patterns emerge.


### LIBRARIES
- **Pandas:** It offers data structures (like DataFrames) for handling and analyzing structured data, particularly for data manipulation and cleaning.
- **Matplotlib.pyplot:** A plotting library used for creating static, interactive, and animated visualizations in Python.
- **NumPy:** It provides support for large, multi-dimensional arrays and matrices, along with mathematical functions to operate on these arrays.
- **Seaborn:** Built on top of Matplotlib, Seaborn simplifies the creation of informative and attractive statistical graphics.

### EXPLORATORY DATA ANALYSIS(EDA)
#### Numerical Data
During the exploratory data analysis of the numerical variables, it was observed that most features exhibited significant skewness, either to the left or right. However, the health and import variables stood out as they followed a normal distribution.
![image](https://github.com/user-attachments/assets/88ff25f4-84aa-4828-8032-d4a799662cc3)

Analyzing the correlation among numerical variables revealed several notable relationships. There is a strong positive correlation of 0.85 between total fertility and child mortality, as well as 0.74 between imports and exports. Additionally, income and GDP per capita (GDPP) show a strong positive correlation. In contrast, life expectancy exhibits strong negative correlations with child mortality (-0.89) and total fertility (-0.76), highlighting significant inverse relationships.
![image](https://github.com/user-attachments/assets/8409da0a-de8e-4865-aa6c-24a239c9293a)

### Data Preprocessing
![image](https://github.com/user-attachments/assets/370e1512-bcdc-4ff0-90e6-0f96ee3699fc)

After performing feature engineering to group all features into three categories—Health, Trade, and Finance—their distributions were analyzed. It was observed that the Health category is left-skewed, the Trade category is right-skewed, and the Finance category follows a normal distribution.
![image](https://github.com/user-attachments/assets/fcbda8ee-0aa3-4ed3-817d-03c0884951dd)

### Model Training
Performed the modeling using the K-Means algorithm and applied the Elbow Method to determine the optimal number of clusters (k).
![image](https://github.com/user-attachments/assets/fff05acc-ee47-4621-af2d-136d3b1f831a)

### Visualisation
Created an interactive GeoMap to visualize the categorization of countries based on their need for foreign aid. The map uses color coding: green represents "Does Not Require Foreign Aid," yellow indicates "Not a Priority," and red highlights "Requires Foreign Aid," aiding in prioritization. The GeoMap reveals that 85% of the countries identified as requiring aid are located in Africa. Additionally, some regions in Europe are categorized as yellow, indicating "Not a Priority," while other areas are marked green, signifying "Does Not Require Foreign Aid."
![newplot](https://github.com/user-attachments/assets/a5072ef0-cddc-42f9-a41f-d0a3abbf40af)

### KEY INSIGHTS
- Most features in the dataset are heavily skewed, with Health metrics left-skewed, Trade metrics right-skewed, and Finance metrics following a normal distribution.
- Strong correlations were observed, such as:
    - Positive correlation between child mortality and total fertility (0.85).
    - Positive correlation between imports and exports (0.74).
    - Negative correlation between life expectancy and child mortality (-0.89).
- Feature engineering grouped variables into three categories: Health, Trade, and Finance, improving model interpretability.
- The Elbow Method determined the optimal number of clusters for K-Means modeling.
- An interactive GeoMap visualized the clustering results:
    - 85% of countries needing aid are concentrated in Africa.
    - Europe showed minimal priority for aid, with most regions classified as "Not a Priority" or "Does Not Require Aid."
- Countries requiring aid exhibit low GDP, high child mortality, and low life expectancy, underscoring the need for targeted interventions in these areas.
  
### RECOMENDATION
- Focus foreign aid efforts primarily on African countries, where 85% of the identified need is concentrated.
- Prioritize funding and resources for countries with low GDP, high child mortality, and low life expectancy to address critical socio-economic and health challenges.
- Implement health-focused interventions, including child mortality reduction programs and investments in healthcare infrastructure.
- Support initiatives to improve trade balance through sustainable exports and reduce reliance on imports in underdeveloped nations.
- Enhance financial stability by promoting economic growth, stabilizing inflation, and increasing income-generating opportunities for low-income populations.
- Collaborate with local governments and organizations in priority countries to ensure efficient distribution of resources and sustainable impact.

## THANK YOU
For more information, you can contact me
![image](https://github.com/user-attachments/assets/fdd843cb-8293-4cca-93c5-856e33770a9b)

