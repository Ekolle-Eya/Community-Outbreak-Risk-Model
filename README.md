# Community-Outbreak-Risk-Model
This project examines the vulnerabilities of communities based on environmental indicators such as number of plastic wastes, drinking water availability, number of hospitals e.t.c. It examines **27 indicators** that can be used to access community risk level in terms of health, water access and resource availability.The dataset for this model involve 72 communities (records).Temperature and Rainfall features are based on climatic condition of the condation based on monthly avearages.

The model provided a core study on how community indicators can influnce a risk to public health, waterborne disease and lack of basic sanitation and hygiene resources
1) This model is built to predict Community Outbreak Risk such as waterborne disease risk, lack of resources and environmental health risk.
2) The model was trained with real data accross **30 communities in 5 countries in Africa and realistic syntethic data all together making up 72 communities**. 
   
Note:"Avg_Toilet_School is the average distance of toilet to the schools in the community", "Avg_Toilet_Household is the average distance of toilet to the households in the community","Avg_Toilet_School is the average distance of toilet to the schools in the community"

[viz](lineplots)
<img width="1230" height="989" alt="Community Indicators for Risk" src="https://github.com/user-attachments/assets/fdb3af4e-0f96-401d-9e05-233f10fa4580" />


### Data
The primary data source used for the machine learning algorithm is the **'comdatarisk_data.csv'** which contained all detailed information. The dataset highlights the interconnectedness of environmental factors and public health risk. it is therefore, a holistic approach that addresses water quality, sanitation, waste management, and access to resources is essential for effective risk reduction and community well-being.

### Tools
1) Google Colab
2) Python
3) Excel

### Data Cleaning and Preparation
The data is clean with no missing values. I clean the data using Excel then use python to perform data inspections and check for correlations and null values to make sure the data is cleaned before proceeding to building the model.

### Exploratory Data Analysis
EDA involve exploring the key independent varaible(Temperature and Humidity) which can have possitive correlation  with the dependent variable 'Water Production_Day'.
Created regression plots of the training data using Matplotlip and Seaborn to evalute linear relationships between variables.

### Machine Learning Algorithms
Random Forest Regression model was use after considering and experimenting on the performance and accuracy of other models such as multiple linear regression

### Model Training
The training involved spliting the data into training set and test with '70%' of the ovarall data allocated for training and '30%' for testing.

### Model Evaluation
Included 5 model evaluation techniques
1) Root Mean Squared Error (RMSE)
2) R-squared (R²)
3) Cross Validation Score (using 5 folds)
4) Added Guasian Noise with random values to evaluate how the model would perform in the case of inaccurate data inputs.
5) Feauture Importance ising SHAP plots- This was use to evaluatre how each features in the dataset influence the predictuion of "Community Risk"
[viz](features)
<img width="797" height="940" alt="Importance of Indicators" src="https://github.com/user-attachments/assets/59c79217-6f79-4a34-872a-54b46afdc6c8" />

### Results
The results of the Random Forest Regression model showed an MSE of 0.0017 and  R-squared of 0.96.The cross validation score produced  R-squared values in 5 folds (0.93508542 0.99649129 0.99790762 0.99816153 0.98188284). With this resutl it is evident that the model can be used in real world applications.

### Conclusion
Base on the Shap plot and line plots it can be seen that several features (community indicators) contributes to determine wether a community is at risk or not. Here, are the following observations and conlutions drawn from this study.

1. **Number of outbreaks**: If a community has already had a alot of outbreaks, it's likely to have a higher risk of more outbreaks or health issues. While, if a community hasn't had many or any outbreak, the risk is lower. So, the history of outbreaks is a major clue to how risky a community is going to be in the future.
2. **Avg. Toilet-Household (m)**: This is about how far people's homes are from toilets. If this distance is larger, it seems to push the community risk higher. Therefore, the more difficult it is to get to a toilet, the more likely sanitation issues could lead to problems such as open defication and sexual violence on girls expecially during night.
3. **Waterborne disease cases**: If a community has had more cases of diseases spread through water, the model sees that and flags the community as higher risk. Therefore, Past waterborne diseases are a strong indicator of future risk.
4. **Number of deaths**: Similar to outbreaks and disease cases, if there have been more deaths, especially likely related to health issues or waterborne disease outbreaks, the model considers the community more risky. Sadly, a higher death count can point to serious underlying health or environmental problems in communities which needs to be address with immediate effect.
5. **Unapproved waste sites**: If a community has more places where waste is just dumped without proper management, the risk goes up. This falitates the spreading of disease and polluting the environment. More unapproved waste means higher risk.
6. **Avg. Water-School (m)**: This is the average distance from schools to water sources. If schools are farther away from water, the risk tends to be higher. Easy access to water at schools is important for hygiene and preventing the spread of illness among children.
7. **Tons of plastic waste**: The amount of plastic waste in a community also plays a critical role. More plastic waste is linked to higher risk. This could be because plastic waste pollutes water sources, clogs drainage, and provides breeding grounds for pests.
8. **Avg. Water-Household (m)**: This is the average distance from homes to water sources. If homes are farther away from water, the risk tends to be higher. Just like with toilets, easy access to clean water at home is crucial for drinking, cooking, and hygiene.
9. **Amount of drinking water consumed**: Communities where less drinking water is available tends to have a higher risk. This could suggest that in higher-risk communities, access to safe drinking water is limited, leading people to consume less or use unsafe sources.

### References
1) Ekolle Eya
2) EKCOLAB Organization
