# Capstone-Project_TTC: Data-Driven Decision Making: Leveraging Classification, Regression, and Predictive Analytics in Analyzing TTC Transportation Delays Data 

**1.1 PROJECT OVERVIEW:**
The efficacy and reliability of public transit systems are pivotal to the socioeconomic fabric of urban environments. Toronto Transit Commission (TTC)- the most heavily used urban mass transit system in Canada and carrying ~319mn riders in 2022, serves as the backbone of the city’s transport network, yet it is frequently beset by delays (~72k standalone incidents/~200 per day in 2023) that disrupt travel plans and contribute to economic losses. This project aims to analyze and optimize the performance of Toronto's public transit system (TTC) by focusing on bus and subway delays. Utilizing techniques in classification, regression, and predictive analytics, the project will identify key factors leading to delays, predict future occurrences, and propose data-driven strategies for minimizing these disruptions.

**1.2 RESEARCH QUESTIONS:**
The scope of this project will revolve around three core research questions. 
1.	What are the primary causes of delays in TTC transportation operations, and how do they vary by time of day, day of the week, and season?
-	This question aims to identify and quantify the main factors that contribute to transit delays, potentially leading to targeted strategies to reduce them.
2.	Can historical delay data be used to predict future delays, and what models provide the best accuracy and reliability for such predictions?
-	This question focuses on predictive analytics, leveraging past data to forecast future occurrences and the effectiveness of different predictive models. 
3.	What mitigation strategies can be developed from the delay data analysis to improve the reliability of TTC services, and how can these strategies be implemented effectively?
-	Lastly, we concentrate on formulating effective mitigation strategies based on our data analysis to enhance the reliability of TTC services.

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

Step 1: Data Collection, Initial Analysis and Preprocessing:
o	Gather historical data of 2021-2023 on TTC bus delays, including time, duration, locations, causes, and affected lines/routes.
o	Clean and preprocess the data for analysis (handling missing values; identify and define dependent/ target variable; assign correct data types, standardize column names, and address inconsistencies; handle outliers and categorical variables with excessive levels; assess distributions of variables; data imbalance to ensure data quality.
o	Utilize visualizations to uncover univariate, Bi-variate and multivariate relationships and apply statistical tools for in-depth analysis.

Step 2: Exploratory Data Analysis (EDA):
o	Conduct thorough exploratory analysis to understand patterns and trends in the data.
o	Visualize delay frequencies, durations, and distributions across different times and routes.
o	Subset data for focused analysis and establish decision rules based on initial findings; Apply clustering techniques to identify patterns and groupings in the data (if required)

Step 3: Data Normalization and Dimensionality Reduction: 
o	Normalize data to ensure uniform scale across variables.
o	Implement feature selection methods to retain impactful variables.
o	Utilize feature extraction techniques to transform data into a manageable size while preserving essential information.

Step 4: Experimental Design:
o	Split the dataset into training and test sets to validate model performance.
o	Apply appropriate treatments for imbalanced data.
o	Use cross-validation techniques to ensure robustness and generalizability of the models.

Step 5: Modelling:
o	Classification Analysis: Classify delays into categories based on their causes (e.g., technical issues, weather conditions, operational problems). Use classification algorithms (like Logistic Regression, Random Forest, Gradient Boosting, K-Nearest neighbours) to identify the most significant predictors of delay types.
o	Regression Analysis: Employ regression techniques like linear regression to analyze factors affecting delay durations. Develop models to quantify the impact of various variables (like time of day, season, route traffic) on delay length.
o	Predictive Analytics: Build predictive models to forecast potential delays and their characteristics using classification and regression machine learning techniques. 

Step 6: Evaluation:
o	Evaluate models using metrics like R-squared, RMSE for regression, and confusion matrix, accuracy, recall, precision for classification.
o	Rigorously test models to ensure accuracy and reliability.

Step 7: Improving the Model:
o	Identify and address any fixation variables affecting model performance.
o	Implement strategies to prevent overfitting.
o	Consider adding more observations for a comprehensive dataset.
o	Adopt an iterative process for continuous model refinement.

Step 8: Conclusions/Recommendations:
o	Draw inferences from the models and analysis, engaging in meaningful discussions on findings.
o	Acknowledge any threats to validity and how they were addressed.
o	Provide actionable recommendations for TTC to reduce delays.
o	Outline next steps for further research or implementation.
In sum, this project enhances Toronto's public transit reliability by using data analytics to unravel bus delay patterns, aiming to predict and pre-emptively mitigate future disruptions.
<img width="468" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/17a93255-4d37-4912-91c4-62399f90eaed">

<img width="468" alt="image" src="https://github.com/DarianSB/Capstone-Project_TTC/assets/145614449/45ff13b1-e436-4afc-8010-f986dd8253bc">
