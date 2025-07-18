 # 🏠Property-price
 __This read me file indicates a breakdown process of obtaining the price of a property(houses) in england.__
 
 __House price prediction is a problem in the real estate industry to make informed decisions. By using machine learning algorithms we can predict the price of a house based on various features such as location, size, number of bedrooms and other relevant factors.  we will explore how to build a machine learning model in Python to predict house prices to gain valuable insights into the housing market.__
 
__To tackle this issue we will build a machine learning model trained on the House Price Prediction Dataset. We can download the dataset from the provided link. It includes 13 features:__

 __I have used google colab as it more efficient and effective ,for its's inbuilt AI features.__
 
 __I have broken down the whole process in to steps, from step 1 to step 7.And the steps are all well explained for an easy follow up.Below are the steps.__

 # Step 1:Importing libraries and Dataset
* I started by importing the necessary libraries required to manipulate the data.As well as    importing the dataset.
* In the above step we go ahead to identify the shape of our dataset,to determine the volume of it which is (2919,13).
* To clearly understand step 1 click here https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150256.png
# Step 2: Data preprocessing
* Now, we categorize the features depending on their datatype (int, float, object) and then calculate the number of them. As shown here https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150408.png
# Step 3: Exploratory Data Analysis
* EDA refers to the deep analysis of data so as to discover different patterns and spot anomalies. Before making inferences from data it is essential to examine all your variables. So here let's make a heatmap using seaborn library.https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150432.png
* We use the heatmap to show the correction between the categorical data 
 https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150451.png
* We need to idenfity how many categorical data we have in our dataseet.https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150549.png
*  Lets visualize the counts of the categorical data we have in our dataset  https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150607.png
*  The plot shows that Exterior1st has around 16 unique categories and other features have around  6 unique categories. To findout the actual count of each category we can plot the bargraph of each four features separately.https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150622.png
*  We then visualize from the code above https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150637.png
# Step 4: Data Cleaning 
* The way to improvise the data or remove incorrect, corrupted or irrelevant data. As in our dataset there are some columns that are not important and irrelevant for the model training. So we can drop that column before training. There are 2 approaches to dealing with empty/null values.
* As Id Column will not be participating in any prediction. So we can Drop it.
* Replacing SalePrice empty values with their mean values to make the data distribution symmetric. https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150702.png
* Drop records with null values (as the empty records are very less).
  https://github.com/HenrySsali/Property-price/blob/main/images/Screenshot%202025-07-15%20150716.png
* Checking features which have null values in the new dataframe (if there are still any).
# Step 5: One Hot Encoder 
* One hot Encoding is the best way to convert categorical data into binary vectors. This maps the values to integer values. By using OneHotEncoder, we can easily convert object data into int. So for that firstly we have to collect all the features which have the object datatype. To do so, we will make a loop.
* Then once we have a list of all the features. We can apply OneHotEncoding to the whole list.
# Step 6: Splitting Dataset into Training and Testing 
* X and y splitting (i.e. Y is the SalePrice column and the rest of the other columns are X)
# Step 7: Model Training and Accuracy 
* As we have to train the model to determine the continuous values, so we will be using these regression models.

* SVM-Support Vector Machine
* Random Forest Regressor
* Linear Regressor
* Support vector Machine is a supervised machine learning algorithm primarily used for classification tasks though it can also be used for regression. It works by finding the hyperplane that best divides a dataset into classes. The goal is to maximize the margin between the data points and the hyperplane.
* Random Forest is an ensemble learning algorithm used for both classification and regression tasks. It constructs multiple decision trees during training where each tree in the forest is built on a random subset of the data and features, ensuring diversity in the model. The final output is determined by averaging the outputs of individual trees (for regression) or by majority voting (for classification).
* Linear Regression is a statistical method used for modeling the relationship between a dependent variable and one or more independent variables. The goal is to find the line that best fits the data. This is done by minimizing the sum of the squared differences between the observed and predicted values. Linear regression assumes that the relationship between variables is linear.


 
