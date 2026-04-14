Task 1

1. Label - "repeat_purchase_flag" can be used as label for this model with its value being 0 by default and 1 if the customer purchases repeat order. 

2. Data Leakage - The column "repeat_purchase_flag" will introduce Data leakage in the model as the column value always directly relates to the desired output from the model. The model will adapt in such a way that during training where ever it will find this column value to be '1', it will give the output that the customer will surely make a repeat purchase. But when an unseen data will be tested on the model where this column value is unknown or '0', the model will directly indicate that the customer will not make a repeat purchase, which might be wrong.

Task 2

Step 1 - Splitting the data into testing and training data is very important because if entire dataset is used for training the model then it will lead to data leakage and the model will be overfitting.

Step 2 - Scaling the data is very important because if any one column will have larger numeric values that others, ML model will become bias into thinking as if that column is more important than others, which might be wrong.