# Community-Outbreak-Risk-Model
This project examines the vulnerabilities of communities based on environmental indicators such as number of plastic wastes, drinking water availability, number of hospitals e.t.c. It examines 22 indicators that can be used to access community risk level in terms of health, water access and resource availability.The dataset for this model involve 72 communities (records).Temperature and Rainfall features are based on climatic condition of the condation based on monthly avearages.

The model provided a core study on how community indicators can influnce a risk to public health, waterborne disease and lack of basic sanitation and hygiene resources
1) This model is built to predict Community Outbreak Risksuch as waterborne disease risk, lack of resources and environmental health risk.
2) The model was trained with real data accross 30 communities in 5 countries in Africa and realistic syntethic data all together making up 72 communities. 
   
Note:"Avg_Toilet_School is the average distance of toilet to the schools in the community", "Avg_Toilet_Household is the average distance of toilet to the households in the community","Avg_Toilet_School is the average distance of toilet to the schools in the community"

[viz](lineplots)
<img width="1230" height="989" alt="Community Indicators for Risk" src="https://github.com/user-attachments/assets/fdb3af4e-0f96-401d-9e05-233f10fa4580" />


### Data
The primary data source used for the machine learning algorithm is the 'comdatarisk_data.csv' which contained all detailed information. The dataset highlights the interconnectedness of environmental factors and public health risk. it is therefore, a holistic approach that addresses water quality, sanitation, waste management, and access to resources is essential for effective risk reduction and community well-being.

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
Included 4 model evaluation techniques
1) Root Mean Squared Error (RMSE)
2) R-squared (R²)
3) Cross Validation Score (using 5 folds)
4) Added Guasian Noise with random values to evaluate how the model would perform in the case of inaccurate data inputs.
5) Feauture Importance ising SHAP plots- This was use to evaluatre how each features in the dataset influence the predictuion of "Community Risk"

### Results
The results of the Random Forest Regression model showed an MSE of 0.0017 and  R-squared of 0.96.The cross validation score produced  R-squared values in 5 folds (0.93508542 0.99649129 0.99790762 0.99816153 0.98188284). With this resutl it is evident that the model can be used in real world applications.

### Recommendations

### References
1) EKCOLAB Organizatio
