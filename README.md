# Capstone-Project_TTC: Data-Driven Decision Making: Leveraging Classification, Regression, and Predictive Analytics in Analyzing TTC Transportation Delays Data 

**1.1 PROJECT OVERVIEW:**
The efficacy and reliability of public transit systems are pivotal to the socioeconomic fabric of urban environments. Toronto Transit Commission (TTC)- the most heavily used urban mass transit system in Canada and carrying ~319mn riders in 2022, serves as the backbone of the city’s transport network, yet it is frequently beset by delays (~72k standalone incidents/~200 per day in 2023) that disrupt travel plans and contribute to economic losses. This project aims to analyze and optimize the performance of Toronto's public transit system (TTC) by focusing on bus and subway delays. Utilizing techniques in classification, regression, and predictive analytics, the project will identify key factors leading to delays, predict future occurrences, and propose data-driven strategies for minimizing these disruptions.

**1.2 RESEARCH QUESTIONS:**
The scope of this project will revolve around three core research questions. 

  **1.	What are the primary causes of delays in TTC transportation operations, and how do they vary by time of day, day of the week,            and season?**
     -	This question aims to identify and quantify the main factors that contribute to transit delays, potentially leading to targeted          strategies to reduce them.
     
  **2.	Can historical delay data be used to predict future delays, and what models provide the best accuracy and reliability for such           predictions?**
     -	This question focuses on predictive analytics, leveraging past data to forecast future occurrences and the effectiveness of              different predictive models. 
     
  **3.	What mitigation strategies can be developed from the delay data analysis to improve the reliability of TTC services, and how can         these strategies be implemented effectively?**
     -	Lastly, we concentrate on formulating effective mitigation strategies based on our data analysis to enhance the reliability of           TTC services.

**1.3 DATA COLLECTION:**
To address these questions, a non-textual dataset obtained from the City of Toronto’s Open Data Portal (Dataset link: https://open.toronto.ca/dataset/ttc-bus-delay-data/) will be utilized. There are three sets of data (excel worksheets) for Bus delay from January 1, 2021, to December 31, 2023. The TTC bus dataset has 151,889 rows/ records: providing a granular view of the frequency, duration, and reasons for TTC transportation delays. In the dataset, each row is a record of the delay-causing incident, and we have the following information as attributes/ columns:

    -	Report date
    -	Route Number (The number of the bus route)
    -	Time of the day
    -	Day (Day of the week)
    -	Location / Station (The location or station of the delay-causing incident)
    -	Incident (The description of the delay-causing incident)
    -	Delay (in minute)
    -	Gap (in minute)
    -	Direction / Bound (where the vehicle heading)
    -	Vehicle (vehicle number)
The data encompasses a comprehensive timeframe, offering a robust foundation for both retrospective analyses and forward-looking predictions.

**1.4 TECHNIQUES AND TOOLS:**
Methodologically, this project will employ a multifaceted analytical approach. The step-by-step approach that will be applied are as follows:

**Step 1: Data Collection, Initial Analysis and Preprocessing:**
   o	Gather historical data of 2021-2023 on TTC bus delays, including time, duration, locations, causes, and affected lines/routes.
   o	Clean and preprocess the data for analysis (handling missing values; identify and define dependent/ target variable; assign              correct data types, standardize column names, and address inconsistencies; handle outliers and categorical variables with                excessive levels; assess distributions of variables; data imbalance to ensure data quality.
   o	Utilize visualizations to uncover univariate, Bi-variate and multivariate relationships and apply statistical tools for in-depth         analysis.

**Step 2: Exploratory Data Analysis (EDA):**
   o	Conduct thorough exploratory analysis to understand patterns and trends in the data.
   o	Visualize delay frequencies, durations, and distributions across different times and routes.
   o	Subset data for focused analysis and establish decision rules based on initial findings; Apply clustering techniques to identify         patterns and groupings in the data (if required)

**Step 3: Data Normalization and Dimensionality Reduction: **
   o	Normalize data to ensure uniform scale across variables.
   o	Implement feature selection methods to retain impactful variables.
   o	Utilize feature extraction techniques to transform data into a manageable size while preserving essential information.

**Step 4: Experimental Design:**
   o	Split the dataset into training and test sets to validate model performance.
   o	Apply appropriate treatments for imbalanced data.
   o	Use cross-validation techniques to ensure robustness and generalizability of the models.

**Step 5: Modelling:**
   o	Classification Analysis: Classify delays into categories based on their causes (e.g., technical issues, weather conditions,              operational problems). Use classification algorithms (like Logistic Regression, Random Forest, Gradient Boosting, K-Nearest              neighbours) to identify the most significant predictors of delay types.
   o	Regression Analysis: Employ regression techniques like linear regression to analyze factors affecting delay durations. Develop           models to quantify the impact of various variables (like time of day, season, route traffic) on delay length.
   o	Predictive Analytics: Build predictive models to forecast potential delays and their characteristics using classification and            regression machine learning techniques. 

**Step 6: Evaluation:**
   o	Evaluate models using metrics like R-squared, RMSE for regression, and confusion matrix, accuracy, recall, precision for                 classification.
   o	Rigorously test models to ensure accuracy and reliability.

**Step 7: Improving the Model:**
   o	Identify and address any fixation variables affecting model performance.
   o	Implement strategies to prevent overfitting.
   o	Consider adding more observations for a comprehensive dataset.
   o	Adopt an iterative process for continuous model refinement.

**Step 8: Conclusions/Recommendations:**
    o	Draw inferences from the models and analysis, engaging in meaningful discussions on findings.
    o	Acknowledge any threats to validity and how they were addressed.
    o	Provide actionable recommendations for TTC to reduce delays.
    o	Outline next steps for further research or implementation.
In sum, this project enhances Toronto's public transit reliability by using data analytics to unravel bus delay patterns, aiming to predict and pre-emptively mitigate future disruptions.

<img width="468" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/17a93255-4d37-4912-91c4-62399f90eaed">

<img width="468" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/45ff13b1-e436-4afc-8010-f986dd8253bc">

** Exploratory Data Analysis **
Table 1: Snapshot of Raw Data in the RStudio
<img width="467" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/d6eb29db-430d-4edd-9cb5-1025163ffe96">
  
Table 2: Structure of Bus Delay Data
<img width="453" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/c16f03b7-a586-4182-9f15-a931979b0c25">

Table 3: Metadata of Bus Delay Data
<img width="341" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/3e0837f8-d94c-4462-a481-fc16e6bc96e9">

Table 4: Summary of Bus Delay Data
<img width="460" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/0bcc168d-199a-467f-b53a-e471e61a9c06">

** 3.2 Data Cleaning and Pre-processing:**
3.2.1 Assigning correct data types:
<img width="460" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/cf26b8b4-dfbc-475d-91ac-9a8801ede256">

3.2.2 Handling Missing Data:
Table 6: Handling Missing Values of Bus Delay Data:
<img width="457" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/b377be84-b802-450c-93e2-7cf6393377ac">
<img width="457" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/8cc5e260-be5b-4b05-a88a-07fe6ebc2805">
<img width="454" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/aec6395f-7419-44a2-a58e-80a25c7b3885">

3.2.3 Identifying and defining dependent/ target variable:
Figure 2: Boxplot of Min Delay by Incident Type:
<img width="461" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/8de19a97-4825-457d-9419-5725a129084c">

Table 7: Grouping “Min Delay” by Incident Type:
<img width="439" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/af9e4ab2-7345-4369-827b-1f4c9ae44be0">
<img width="439" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/9443ddef-0ae0-47df-b49b-037106470e22">

3.2.6 Analyzing Data Imbalance:	
Figure 4: Distribution of ‘Delay Severity’:
<img width="468" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/5c5c43cd-62d4-428e-bb68-46e0586683bd">

Table 8: By Incident Type Count of ‘Min Delay’ and Percentage of Total:
<img width="467" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/565fce12-94ed-4d66-9a88-accbe32c4967">

3.2.7 Categorical Variables with Excessive Levels:
Figure 5: By Time Period Count of Grouped ‘Min Delay’:
<img width="430" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/659bc721-5001-4797-b46c-fa145f42a512">

Figure 6: Boxplot of Delay Distribution by Delay Severity:
<img width="421" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/13e2579e-b768-4d6c-92aa-6e249f14f420">

Figure 7: Bar Graph Visualization of By Incident Type Count of ‘Min Delay’:
<img width="403" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/fd267457-d9ce-43fa-84b3-0d14f0523271">

Figure 8: By Incident Type Count of Grouped ‘Min Delay’:
<img width="416" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/51038706-af54-4382-8534-b74fa5fe4c59">
<img width="453" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/426e663c-d579-4548-a9cf-ab073aee3056">

4.1. Features Correlation Matrix:
Figure 9: Feature Correlation Matrix
<img width="398" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/3fef5598-3aa1-47dd-9619-079b26c3ec06">

4.2. Bus Delay Analysis Across Different Time Periods:
Figure 10: Delay Analysis by Month
<img width="468" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/04c3f8a6-d323-4216-a8c3-0d8553b6c7c7">

Figure 11: Average Delay Scenario by Day:
<img width="468" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/2689553f-e445-4919-a563-515b78f28eb9">

Figure 13: Boxplot of Delay Distribution by Time-period
<img width="470" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/54282d5e-548b-4b71-8bbc-c496995b3712">

Figure 14: Trend of Total Incidents Over last 3 Years
<img width="445" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/f58bb1a8-eb5f-461d-8da3-63f556689445">

4.3. Delay Analysis Based on Geographic Location and Incident Type:
Figure 15: Top Routes with Highest Delay
<img width="463" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/83721203-526c-4567-ab26-5560a74833dd">

Figure 16: Top Locations with Highest Delay
<img width="378" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/addcffc1-4e19-4eb4-b98e-e05f33ddee8c">

<img width="464" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/d7fd92c6-4592-4c60-9233-b650f7e38af8">

CHAPTER 5: ‘DIMENSIONALITY REDUCTION’ AND ‘DATA NORMALIZATION:

5.1. Applying Linear Regression to Understand Significant Predictors:

Figure 9: Identifying Significant Predictors through Linear Regression:
<img width="257" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/e9ca9bff-c47b-49d9-b4d9-93a63139073a">

5.2. Applying Dimensionality Reduction Techniques:
Table 9: Outcome of Forward Selection: 
<img width="436" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/cb4e56a2-d6f4-438f-b107-fce885823010">

Table 10: Outcome of Backward Elimination: 
<img width="470" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/b54ca2c6-7e69-4d98-b916-200bf1403a7f">

5.3. Data Normalization for ML Modelling: 
Table 11: Data Normalization Outcome:
<img width="419" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/18d60c16-c97f-437a-b3de-b2fe80ba5217">

** CHAPTER 6: MACHINE LEARNING MODELLING FOR BUS DELAY PREDICTION **
This section introduces the building of bus  delay prediction models and their optimization. The machine learning model/ algorithms predicts the delay severity based on 3 prediction classes: 
-	Borderline Late (<10 Min)
-	Considerably Late (10-15 Min)
-	Extremely Late (>15 Min)






























