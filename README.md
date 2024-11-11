**Group 10 _ Boston Housing Dataset**
* Subject: Data Science
* Lecturer : Dr. Emmanuel Lance Christopher VI M. Plan
*  Evaluation Of Teamwork
  
 | Tên        | Mã Sinh Viên  | Task Done| Evaluation|
 |:-----------|-----:|---|---|
 | Nguyễn Quang Anh   | 22080296   | Correlation Heatmap of Features chart| 100%|
 | Triệu Anh  | 22080299   | KNN model & slide| 100%|
 | Nguyễn Tú Anh  | 22080346   | Introduction, Data Source,Preparation and Cleaning & Conclusion|100%|
 | Lê Quý Quỳnh Chi  | 22080305   | Logistic Regression|100%|
 | Nguyễn Khánh Duy   | 22080310   | Liner Regression and slide|100%|
 | Nguyễn Hải Đăng  | 22080307   | Histogram chart|100%|







1.**Introductions**:


  ![ảnh gth](https://github.com/user-attachments/assets/b649ccb2-294c-44af-9b85-0be884c9c698)
  

The Boston Housing Dataset is a classic dataset widely used in machine learning, particularly for regression tasks. It provides a set of features describing housing values in different neighborhoods in Boston, Massachusetts, and is commonly used to predict the median value of owner-occupied homes based on various factors.

Purpose: The dataset is used to predict the median value of homes in Boston, making it ideal for regression models.

Context: The data originates from the 1970 U.S. Census and was collected for studying factors that affect home prices in different areas of Boston.

Size: The dataset consists of 506 samples (data points), with 14 variables in total, including 13 features and one target variable.

2.**Data Source**

Original Source: The data comes from the 1970 U.S. census and was originally used in statistical research at the StatLib repository, maintained by Carnegie Mellon University.

Kaggle: https://www.google.com/url?q=https%3A%2F%2Fwww.kaggle.com%2Fdatasets%2Fkrupadharamshi%2Fbostonhousing

The dataset consists of 13 numeric features that describe various aspects of housing and the environment. Each feature corresponds to a specific aspect of the neighborhood or house being studied:

**CRIM**: Crime rate per capita in the neighborhood.

**ZN**: Proportion of residential land zoned for large lots (over 25,000 sq. ft.).

**INDUS**: Proportion of non-retail business acres per town (percent of town's land dedicated to industrial use).

**CHAS**: Charles River dummy variable (1 if the property borders the river, 0 otherwise).

**NOX**: Nitrogen oxide (NO) concentration (in parts per 10 million).

**RM**: Average number of rooms per dwelling.

**AGE**: Proportion of owner-occupied units built before 1940.

**DIS**: Weighted distance to employment centers (such as downtown Boston).

**RAD**: Index of accessibility to radial highways.

**TAX**: Property tax rate per $10,000.

**PTRATIO**: Pupil-teacher ratio by town.

*B*: Proportion of residents of African American descent.

**LSTAT**: Percentage of the population classified as "lower status.

Target Variable:

**+MEDV**: Median value of owner-occupied homes in thousands of dollars (the target variable to predict).
![Screenshot (169)](https://github.com/user-attachments/assets/5205d0a9-9e3a-446a-a638-d7518af68cbe)

![Screenshot (170)](https://github.com/user-attachments/assets/be57e90d-7ddd-493e-bfce-245b402b1070)



3.**Preparation and Cleaning**

The preparation and cleaning steps help optimize the data for predicting housing prices based on features like **crim** (crime rate), **rm** (number of rooms), **age** (building age), **chas** (location near the Charles River), **dis** (distance to employment centers), and others. This enables the model to accurately learn relationships between the features and housing prices, thus making reliable predictions for prices in various areas.

**Shape and Data Overview**
- Total Entries: There are 506 rows, indicating 506 observations or instances in the dataset.
- Total Columns: There are 14 columns, representing different features or variables that can help in predicting housing prices.

**Column Names and Data Types**
- The columns are labeled from crim to medv. All of them has '506 non-null' values, so that there are no missing values in this dataset, which simplifies the data preparation process.
- Data Types:
'float64': Eleven columns are of type 'float64', meaning they contain numerical values with decimal points. These columns are 'crim', 'zn;, 'indus', 'nox', 'rm', 'age', 'dis', 'ptratio', 'b', 'lstat', and 'medv'.
'int64': Three columns are of type 'int64', which store integer values. These are 'chas', 'rad', and 'tax'.

4.**Chart**

 
   4.1 **Histogram Matrix**
   



  ![ảnh chart1](https://github.com/user-attachments/assets/93ee5b7b-0077-4f1c-8fb9-5b3e9b55b13d)

- **crim** (Crime rate per person):

Most areas have low crime rates (below 10), and the most common value is under 2.
There are a few areas with very high crime rates (over 20 and even up to 80), but these are rare and stand out from the rest.
- **zn** (Percent of residential land with large lots):

In most areas, this value is 0, meaning that very few areas have large lots (over 25,000 sq.ft).
Only a small number of areas have values above 80, so big lots are uncommon.
- **indus** (Percent of land for industry):

This mostly stays below 20, with the peak around 10.
Only a few areas go above 20, meaning that most towns don’t have much industrial land.
- **chas** (Near the Charles River or not):

This is a yes-or-no variable. Most areas are not near the river (value 0), and only a small number are (value 1).
So, proximity to the Charles River is uncommon.
- **nox** (Air pollution - nitric oxide levels):

Most values are between 0.4 and 0.7, with the peak around 0.5.
A few areas have higher pollution (close to 0.8), but these are unusual.
- **rm** (Average number of rooms per house):

Most houses have between 5 and 7 rooms, with the peak at around 6.
Only a few areas have houses with less than 4 or more than 8 rooms, meaning most homes have a similar size.
- **age** (Percent of houses built before 1940):

Most values are near 100, meaning many houses are old (built before 1940).
Only a few areas have values below 20, showing that newer homes are rare.
- **dis** (Distance to job centers in Boston):

Most values are between 1.5 and 3, meaning most areas are pretty close to jobs in Boston.
Some areas are farther away (values over 10), but these are not common.
- **rad** (Access to highways):

There are distinct clusters here, with one big peak around 1 and a smaller peak at 24.
This means some areas have very easy highway access, while others do not.
- **tax** (Property tax rate per $10,000):

Most values are between 200 and 400, with a small group around 700.
This suggests that most areas have mid-level taxes, but some have very high taxes.
- **ptratio** (Pupil-teacher ratio):

Values mainly range from 15 to 20, with a peak at 18.
The ratio is pretty consistent across areas, without major differences.
- **b** (Proportion of Black residents in town):

Most values are high (around 400), meaning many towns have a high proportion of Black residents.
A few values are below 100, showing some areas have a lower proportion of Black residents.
- **lstat** (Percent of low-income population):

Most values are below 20%, with a peak around 10%.
Only a few areas have a high percentage of low-income residents (over 30%), so these areas are not common.
- **medv** (Median home value in $1,000s):

Most values are between 15 and 30 thousand dollars, with a peak around 20.
Some areas have high home values over 50 thousand dollars, but these are rare.

 **Summary**
 - Right-skewed distributions: Variables like crim, zn, dis, b, and lstat have right-skewed distributions, meaning that most values are low, but there are a few high values that stand out.
 - Almost normal distributions: Variables like rm (average rooms) and medv (median home value) are nearly normal, showing that most values are around the average.
  - Binary variable: chas is binary (0 or 1), where most values are 0, indicating that few areas are near the Charles River.
 - Clusters: Variables like tax, ptratio, and age are tightly clustered around certain values, which could reflect specific policies or features of the area.


Understanding these patterns gives us insight into what each area is like in the Boston Housing dataset and helps us see which factors might affect home values (medv).


   4.2 **Correlation Heatmap of Features**




  ![ảnh chart2](https://github.com/user-attachments/assets/823e1d46-6d31-4584-b38b-9b29a52ab719)
  

**Data Analysis and Graphing**:

1. **Heatmap**: This graph displays the correlation coefficients with a colour scale, making it easy to see which relationships are strong and which are weak:

• Red represents a strong positive correlation (close to 1).

• Blue represents a strong negative correlation (close to -1).

• Values ​​in the middle (close to 0) represent weak or no clear relationship.

2. **Examine the Correlation Coefficients**:

**crim** (crime rate):

* Strong positive correlation with rad (proximity to freeways) (0.63) and tax(taxes) (0.58), meaning that high-crime areas tend to have high road density and high taxes.

* Negative correlation with dis(average distance to employment centers) (-0.38), indicating that high-crime areas tend to have long distances to employment centers.

**zn** (proportion of lots larger than 25,000 sq. ft.):

* Strong negative correlation with indus(industrial land) (-0.53) and nox(pollution concentration) (-0.52), indicating that industrial and air-polluted areas tend to have fewer large lots.

* Positive correlation with dis(average distance to employment) (0.66), indicating that areas with large lots are generally located further from employment centres.

**rm** (average number of rooms per house):

* Strong positive correlation with medv(house value) (0.7), meaning that houses with more rooms are generally more valuable.

* Negative correlation with lstat(low-status population proportion) (-0.61), indicating that areas with a high proportion of low-income people tend to have fewer rooms per house.


3. **Summary**

* Low-status residents and high student-teacher ratios tend to be in areas with low home values.

* High pollution in industrial areas near employment centers.

* Access to freeways is associated with higher taxes.

4.3 **KNN**




  ![ảnh chart 3(1)](https://github.com/user-attachments/assets/7f8c56da-3c02-4922-bd97-dd1ee5f75d0a)


  
  ![ảnh chart3(2)](https://github.com/user-attachments/assets/0753533a-49fe-45b9-980f-ccb2a171ff33)


  The first thing we aim to do with this model is to classify house prices into two groups based on the median value of 'medv'. This helps determine whether the house price in the dataset is above or below the average level. Therefore, in this model, I use "Binary Classification KNN" to clearly classify house prices as either high or low. I selected six main factors that influence house prices:

**RM**: average number of rooms per dwelling

**PTRATIO**: pupil-teacher ratio by town

**LSTAT**: lower status of the population

**INDUS**: proportion of non-retail business acres per town

**NOX**: nitric oxides concentration (parts per 10 million)

**TAX**: full-value property tax rate per $10,000

These features not only have a strong correlation with house prices (Correlation Heatmap of Features) but are also key factors affecting prices.

Although K could be 9, the accuracy is not as good as when K is 8, so we decided to choose K = 8.

Here, we chose a value of K = 8 to create a balance between overfitting and underfitting. If k is too small (such as 1 or 3), the model will be sensitive to noise as it relies on only a few neighboring points, leading to overfitting.

To find the best K value, we used the "cross-validation" method, where we tested multiple values of k and selected the one with the highest accuracy."

To build this model, we had to standardize the data. The important features in the data have different units and ranges, so we used StandardScaler to transform these key features to a scale with a mean of 0 and a standard deviation of 1. This helped the model make better evaluations.

The model performed quite well, achieving an accuracy of 85.3%, indicating that the model correctly classified 85.3% out of 100% of the cases. High accuracy is a sign that the selected features are valuable in classifying house prices into 'Low' and 'High' categories.

Confusion Matrix:

* True Positives (TP): 51 - The number of 'Low' cases correctly predicted.
* False Positives (FP): 7 - The number of 'Low' cases mistakenly predicted as 'High'.
* True Negatives (TN): 36 - The number of 'High' cases correctly predicted.
* False Negatives (FN): 8 - The number of 'High' cases mistakenly predicted as 'Low'.
The model works well with both groups but still has some confusion between the 'Low' and 'High' groups, especially in cases where 'High' was predicted as 'Low' (FN = 8).

Classification Report: Precision and Recall: The precision and recall for both 'Low' and 'High' groups are quite high.

* Precision for the 'Low' group is 0.86, and for the 'High' group is 0.84.
* Recall for the 'Low' group is 0.88, and for the 'High' group is 0.82.
F1-Score: Both groups have high F1-Scores (above 0.8), indicating that the model achieves a good balance between precision and recall. However, the 'Low' group has a slightly higher F1-Score, which may be due to the model finding it easier to distinguish lower-priced houses.

**Summary**

* The model provides an overview and performs quite well in classifying house prices as "High" and "Low." The effectiveness of the model shows good results in selecting the six main factors that influence house prices based on medv. However, there are still some errors in predicting the data, with misclassifications possibly occurring due to overlapping characteristics between the two groups or noise in the data.

  4.4.**Linear Regression**


  
    ![ảnh chart4](https://github.com/user-attachments/assets/1a6ed7f9-5d4f-4133-84ea-34319e258a5d)
  

  1.General assessment:

Linear relationship: The graph shows a linear relationship between the actual value and the predicted value of the house price. This means that the model has captured the general trend of the data.

Data dispersion: The data points are relatively evenly dispersed around the regression line, but there are still some points that deviate further. This shows that the model can explain a significant part of the fluctuations in house prices, but there are still some other factors that are not fully modeled.

  2. Assessment of indicators:

Mean Squared Error (MSE): 24.291119474973513: This is the mean squared error, indicating the average degree to which the predicted values ​​deviate from the actual value. The lower the MSE value, the better the model. In this case, the MSE value is relatively low, indicating that the model has quite good accuracy.

R-squared (R2): 0.668759493535632: This is the coefficient of determination, indicating the proportion of variation in the dependent variable (house price) explained by the independent variable (factors affecting house price). The higher the R2 value, the better the model. In this case, the R2 value is 0.668, meaning that the model explains about 66.8% of the variation in house price.

  3. Detailed comments:

-Strengths of the model: The model has captured the general trend of the data, which can be used to predict house prices relatively accurately.
-Limitations of the model:

+Outliers: Some data points located far from the regression line can affect the accuracy of the model.

+Other factors: The model only explains about 66.8% of the variation in house price, which means that there are many other factors that have not been included in the model such as location, area, number of rooms, amenities, etc.

+Linearity: The model assumes that the relationship between variables is linear, when in reality the relationship may be more complex.

4.5.**Logistic Regression**

- From the information of the Correlation Heatmap of Features which present by Quang Anh. We can see that the correlation betwen "nox" and "dis" is -0.77.It indicating a strong negative relationship. This means that as the concentration of nitrogen oxides (nox) increases, the distance to employment centers (dis) tends to decrease, and vice versa.

- The high level of nitrogen oxides are often in urban areas which near the employment centers. And on the other hand, areas with lower pollution levels often in countryside which far from the employment centers. So that I use "nox" and "dis" as Feature (X) and 'Price based on region' ( binary classification based on medv)

- 1 indicates that the property value (medv) is greater than or equal to the median.
- 0 indicates that the property value (medv) is below the median.

![z6022337402997_e045c3d992235e10cd11abf27e1b1a16](https://github.com/user-attachments/assets/2e73b561-207a-4ee0-b612-59625d168b5f)

- High-Price Areas (Price_based_on_region = 1): Here, nox values are generally moderate to low (0.458, 0.469, 0.524), and dis values are moderate to low (4.0900 to 5.9505). This suggests that high-price areas need not only to be close to job centers but also to have moderate or low pollution levels. When dis is low (closer to the center), a moderate level of pollution may be tolerable for buyers.

- Low-Price Areas (Price_based_on_region = 0): In these areas, dis values are generally higher (6.3467, 6.5921), meaning these locations are farther from job centers, which likely affects home prices more than pollution levels. Some areas with higher nox values, such as 0.538, also tend to have lower prices, especially when dis is high. This aligns with the idea that areas both far from job centers and with high pollution levels attract fewer buyers, resulting in lower prices.

- Conclusion
DIS plays an important role in determining high or low home prices. When dis is low (closer to job centers), the area is more likely to be classified as high-priced.
NOX acts as a supplementary factor: when nox is low or moderate in areas closer to job centers (dis is low), home prices are typically higher. The combination of low nox and low dis often leads to higher home prices, whereas high nox and high dis together tend to result in lower prices.
So the house price in urban areas tends to be higher than house price in countryside.


![Screenshot (166)](https://github.com/user-attachments/assets/15f9cac4-ab37-4494-ac2f-e2669b6e91e2)


   
- The accuracy of the model is approximately 68.63%. This means that the model correctly classifies 68.63% of the test samples
- Confusion Matrix
The confusion matrix is:

 [[31 23]

 [ 9 39]]

 31: True Negatives (correctly predicted as low price).

 23: False Positives (incorrectly predicted as high price).

 9: False Negatives (incorrectly predicted as low price).

 39: True Positives (correctly predicted as high price).

- This matrix shows that the model performs better in predicting high prices (Price_based_on_region = 1), with relatively high true positives and low false negatives, but has some difficulty in distinguishing low prices, as indicated by a higher number of false positives.

- The F1 score is 0.71. The F1 score combines both precision and recall to give a single measure of model performance. A score of 0.71 indicates a moderate balance between precision and recall. This score is somewhat consistent with the accuracy, indicating that the model has a fair balance between identifying high and low prices.

- Classification Report report provides precision, recall, and F1-score for each class:
 - Class 0 (Low Price)
Precision: 0.78 – Of all samples predicted as low price, 78% were correct.
Recall: 0.57 – Out of all actual low price samples, the model correctly identified 57%.
F1 Score: 0.66 – This balance of precision and recall results in a moderate F1 score.
 - Class 1 (High Price)
Precision: 0.63 – Of all samples predicted as high price, 63% were correct.
Recall: 0.81 – Out of all actual high price samples, the model correctly identified 81%.

 - F1 Score: 0.71 – This balance of precision and recall for high prices is slightly better than for low prices.
Overall Performance:
The macro average (average of both classes) gives an F1 score of 0.68, which shows that the model's performance is relatively consistent across both classes.
The weighted average also shows similar values, confirming the model is relatively balanced but has better performance in predicting high prices.
- AUC (Area Under the ROC Curve) AUC value is approximately 0.746.
AUC values range from 0 to 1, where a value closer to 1 indicates a strong model that is good at distinguishing between classes. Here, 0.746 suggests the model has a moderate ability to differentiate between high and low prices.
This AUC value indicates that there is some predictive power, but there is room for improvement to make the model even more effective.

-  ROC (Receiver Operating Characteristic) curve visually represents the trade-off between the true positive rate (sensitivity) and the false positive rate for different threshold settings.

The blue curve in the plot shows the model’s performance, while the dotted line represents a random classifier with no predictive power.
Since the blue curve is mostly above the dotted line, the model performs better than random guessing. However, the curve does not fully reach the top-left corner, indicating that while the model can distinguish between high and low prices, it’s not perfect.

  **Summary**
  
- Strengths: The model performs reasonably well, with higher accuracy and good recall, especially for predicting high prices.
- Weaknesses: The model struggles with predicting low prices, as shown by the lower recall for class 0 and a higher number of false positives.


5.**Conclusion:**

- Correlation  Between Different Factors: Factor such as  crime rate, population density, tax rate, and pollution levels clearly affect house prices. From the charts, we see that areas with lower crime, closer to the urban center, and houses with more rooms usually have higher home values.

- Importance of Environment and Location: Factors like distance to job centers, pollution levels, and access to highways or major roads also impact house prices. Even if an area is far from the center, being close to major transportation can keep property values high because it makes commuting easier.

- Useful Insights: This analysis helps us understand how economic, social, and environmental factors work together to affect home values. This information can help  city planners, real estate developers, and investors make better decisions about where and how to develop or invest in different areas.

-> **Overall Conclusion**: The data and charts show that property values depend not just on location but on a mix of environmental and social factors. To predict house prices, it’s important to understand both the market and the specific characteristics of each neighborhood.


















         
 
  


