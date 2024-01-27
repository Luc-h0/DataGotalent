# Programming for Data Science Final Project

## I. Team members information:

- **Class:** 21KHDL
  
    StudentID|Full Name
    -|-
    21127175|Le Anh Thu
    21127693|Huynh Duc Thien


- **Working Plan:** [Trello](https://trello.com/b/eya5drhR/main)

    <img src="Image/Trello.png">

## II. Project information:
### 1. Dataset
Heart failure, a common consequence of Cardiovascular diseases (CVDs), is addressed in this [dataset](#https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction), encompassing 11 distinct features that enable the prediction of potential heart disease.

### 2. EDA
- **Column Meaning**
  
    <img src="Image/Column-meaning.png">

- **Column Types**

    <img src="Image/Column-type.png" height=250>

- **Distribution**
    - Numeric Values
      
    <img src="Image/Numeric-values.png">

    - Categorical Values
      
    <img src="Image/Categorical-values.png">

### 3. Asking Meaning Questions
**a. Question 1:** How does the incidence of heart disease vary across different age groups and genders? 

**Benefits:** This insight facilitates the development of targeted and personalized healthcare interventions for each age group and gender, leading to more effective health outcomes.

**How to answer this question:**

- Analyzing the impact of `Sex` and `Age` on `Heart Disease`
  
    <img src="Image/Age-Sex.png">

- Detail on `Sex`
  
    <img src="Image/Sex.png">

- Detail on `Age`
  
    <img src="Image/Age.png">
    
    <img src="Image/Age-distribution.png">

**&rarr; Answer the question:** How does the incidence of heart disease vary across different age groups and genders?

- **Gender Distribution:**

    Among individuals with heart disease, the data shows a higher prevalence among males (63.2%) compared to females (25.9%). This suggests a notable gender disparity in the incidence of heart disease in the dataset, with males being more affected.

- **Age Distribution:**

    The age distribution indicates a higher prevalence of heart disease in the 55+ age group. This implies that as age increases, the likelihood of having heart disease also increases. Therefore, heart disease appears to be more prevalent among older individuals.
  
<hr/>

**b. Question 2:** Analyze the impact of factors directly related to blood and circulatory system on the risk of developing heart disease. Among these factors, which one has a significant influence and needs to be prioritized? 

**Benefits:** This analysis provides a basis for informed decision-making in heart care and prevention. Moreover, identifying the most influential factor informs the development of tools such as heart rate monitors, aiding in early detection of irregularities. 

**How to answer this question:**

- Analyzing the distribution of `RestingBP`, `Cholesterol`, `FastingBS`, `MaxHR` on `HeartDisease`
  
  <img src="Image/Factors-distribution.png">

- Training `Random Forest Classifier` to evaluate feature importance 
 
  - Classification Report
    
    <center>
    <img src="Image/Classification-report.png" width=350>
    </center>

  - Value Importance
    
    <center>
    <img src="Image/Value-importance.png" width=150>
    </center>
    
    <img src="Image/Feature-importance.png">

**&rarr; Answer the question:** Analyze the impact of factors directly related to blood and circulatory system on the risk of developing heart disease. Among these factors, which one has a significant influence and needs to be prioritized?

- Among the factors directly related to the blood and circulatory system, **Maximum Heart Rate (MaxHR)** emerges as the most influential and significant predictor of heart disease. Both visual analysis and model importance highlight the pronounced impact of MaxHR on the risk of developing heart disease. 
