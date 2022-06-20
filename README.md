# Predicting_NewYork_houseprices_2015

In this notebook Ridge regression and Lasso regression is done to assess the accuracy of predicting house prices. The objective here is to assess wether the image data from sales_data_2015_DF-inception-conv.csv shows a big increase in predictive power. First the data from sales_data_2015.csv is explored in a data analysis. Then progressively features are scaled appropriately using scalers. This also goes for the image dataset sales_data_2015_DF-inception-conv.csv. The idea is that if you take a photo from the house from above that you can enhance predictive power in the price. After this categorical variables are made into dummies.

Lastly the data is split into a train, validation and test set. It is then analysed using cross fold validation. A noticeable conclusion is that Ridge is seemingly having more power with a R^2 score of ~0.42 oppossed to Lasso's ~0.34. Both scores predictively are rather low. It is observed that even with a very low alpha of 0.01 a lot of features, especially those of the image dataset get penalized to 0 in Lasso regression. It can be said that so many features that add almost no value are a poor selection of features and that the image data's predictive power is rather low.

data is available here: https://onedrive.live.com/?id=DF3D4CFD086B9DF1%21231&cid=DF3D4CFD086B9DF1
