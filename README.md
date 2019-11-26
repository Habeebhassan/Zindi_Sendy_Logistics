# Zindi_Sendy_Logistics
Predictive analysis of logistics company's datasets

Zindi called for a competition, in collaboration with Sendy - A logistics platform, that transports consumers' product from one location to another.

The challenge is to build a model that can accurately predict estimated time of arrival for orders from pick-up to drop-off

During data cleaning time variables are in realtime format (H:MM:S PM), so what i did was to convert this format into 24 hours time factor. Some variables are in categorical format with high cardinality. LabelEncoding this variable might increase the dimensionality of the dataset. Therefore, after i discovered that, the these variables are statistically insignificant, i removed them. 

So far i used LinearRegression library from sklearn to predict time it take to transport goods from A to B, using Relative Mean Squared Error (RMSE) metrics to check how close the model is to ground truth.
