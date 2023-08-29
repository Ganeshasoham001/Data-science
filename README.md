# Data-science
1.Flipkart Discount Price Prediction
In this Project I used Kaggle Flipkart datasets which is having 13 Columns and about 20,000 rows
What I have done:
1.Cleaning the dataset which is done in some process
drop unrelated columns and find co relation matrix to see some related columns that is goint to be used in model fitting
the columna which I made at last are(Columns: [retail_price,discounted_price, is_FK_Advantage_product, product_rating, overall_rating, brand, Catagory])
to do this Product Catagory tree which I have used. But it have some clomplicated entries so I have removed first "<<" and make a datatset then we concat only first entry and named it as Catagory
We convert is_FK_Advantage_product True to 1 and False to 0 and convert product_rating and overall_rating into float values which was before string then the entries which was not there we use Mean
inpute where the entries are not given.Then To make it fit for model we use Label Encoder to conver brand and Catagory values to dummy values
2.Train,Test,Split
we make Train,test,split and drom column discounted_price from X dataframe
y data frame is only discounted_price
3.Model selection
I try so many models but the accuracy of Randomfoest Classification worked well.
Result:
After training and testing the model it works quite good give test accuracy about 98.4%
Make a dataframe where user can check it with their determined values
