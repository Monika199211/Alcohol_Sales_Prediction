#### Alcohol Sales Prediction
1.Introduction: There has always been a need by the business owners to know the demand for their products. This benefits the whole business model as it stockpiles the revenue. This improved model deals with the prediction of the consumption of different alcoholic beverages. Based on liquor sales data, various Machine Learning algorithms are applied for enhancing the accuracy of the prediction. The risk of entering a new market can also be minimized by using this model. It is built in a robust way that can be implemented around various fields for improved accuracy in prediction models. We will be using the open-source dataset which is provided by <b> Alcoholic Beverages Division of IOWA Department of Commerce for liquor sales prediction.</b>

2. Dataset Selection
There are lots of different datasets available for alcohol sales prediction. In this research, we have used the dataset which is provided by Iowa Department of Commerce, Alcoholic Beverages Division. Please find the link below:
<a href="https://data.iowa.gov/Sales-Distribution/2019-Iowa-Liquor-Sales/38x4-vs5h">https://data.iowa.gov/Sales-Distribution/2019-Iowa-Liquor-Sales/38x4-vs5h</a>
The dataset size is 549MB with 2.38M million rows and 24 columns. The columns of the datasets are as follows:
  <li>Invoice/Item Number: The unique invoice number.</li>
  <li>Date: The date of liquor purchased or sold.</li>
  <li>Store Number: The store number of the liquor shop.</li>
  <li>Store Name: The store name of the liquor shop.</li>
  <li>Address: The store address of the liquor shop.</li>
  <li>City: City of the liquor shop.</li>
  <li>Zip Code: Zip code of the city.</li>
  <li>Store Location: Liquor store location.</li> 
  <li>County Number: The number of counties.</li>
  <li>County: The county of the liquor sold.</li>
  <li>Category: Category of the liquor.</li>
  <li>Category Name: Category name of the liquor.</li>
  <li>Vendor Number: Vendor number who sold the liquor.</li>
  <li>Vendor Name: Vendor name who sold the liquor.</li>
  <li>Item Number: Unique item number for liquor.</li>
  <li>Item Description: Liquor description.</li>
  <li>Pack: The pack sold out.</li>
  <li>Bottle Volume (ml): The volume of liquor bottles sold in a milliliter.</li>
  <li>State Bottle Cost: The cost of the bottle at the state level. </li>
  <li>State Bottle Retail: The cost of the bottle at the retail level.</li>
  <li>Bottles Sold: Number of bottles sold.</li>
  <li>Sale (Dollars): Sales of liquors in dollars.</li> 
  <li>Volume Sold (Liters): Volume of liquor sold in liters.</li> 
  <li>Volume Sold (Gallons): Volume of liquor sold in gallons.</li>


2. Data Preprocessing
Once the dataset is extracted, there were several issues with the data before it can go for further analysis. Data cleaning and transformation according to the proposal needs to be configured. All the rows with null values should be deleted from the data, dropping duplicate rows. Feature extraction should be kept in mind in this stage of KDD. Although the size of the liquor data is huge, but by data preprocessing standards it should be cleaned appropriately so that we can analyze the data accordingly.

3. Data Transformation or Data reduction and projection
In this stage, the data undergoes major changes to suit the goal of the research. Feature extraction is applied in this stage which means only relevant data is chosen for analysis.

4. Data Visualization and Exploration
Data visualization is an important part of the any machine learning model that we build. The visualization gives us more ideas about the distribution of data and insights of data. The visualization can be any type of graphs, charts, and so on. In Python, there are various libraries available for the visualization of the data.

5. Machine Learning Models
As we are dealing with predicting the sales of alcohol which is a continuous variable that can have any value. So it is a regression problem if we talk in terms of ML terms. The following ML algorithms are applied to the dataset after preprocessing and cleaning. 
•	Ridge regression
•	Random Forest
•	XGBoost


6. Accuracy and Error rate: 
<li> Mean Squared Error : Mean Squared Error is one of the most preferred metrics for regression tasks. It is simply the average of the squared difference between               the target value and the value predicted by the regression model. As it squares the differences, it penalizes even a small error which leads to over-estimation of how           bad the model is. It is preferred more than other metrics because it is differentiable and hence can be optimized better.</li>
        
<li> Root Mean Squared Error: RMSE is the most widely used metric for regression tasks and is the square root of the averaged squared difference between the target               value and the value predicted by the model. It is preferred more in some cases because the errors are first squared before averaging which poses a high penalty on large         errors. This implies that RMSE is useful when large errors are undesired.</li>
        
<li> Mean Absolute Error
MAE is the absolute difference between the target value and the value predicted by the model. The MAE is more robust to outliers and does not penalize the errors as             extremely as MSE. MAE is a linear score which means all the individual differences are weighted equally. It is not suitable for applications where you want to pay more           attention to the outliers</li>.
        
<li> R² Error
Coefficient of Determination or R² is another metric used for evaluating the performance of a regression model. The metric helps us to compare our current model with a           constant baseline and tells us how much our model is better. The constant baseline is chosen by taking the mean of the data and drawing a line at the mean. R² is a               scale-free score that implies it doesn't matter whether the values are too large or too small, the R² will always be less than or equal to 1. </li>
        
<li> Adjusted R²
Adjusted R² depicts the same meaning as R² but is an improvement of it. R² suffers from the problem that the scores improve on increasing terms even though the model is         not improving which may misguide the researcher. Adjusted R² is always lower than R² as it adjusts for the increasing predictors and only shows improvement if there is a         real improvement. 
