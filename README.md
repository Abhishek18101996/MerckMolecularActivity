# MerckMolecularActivity

This project aims to predict the biological activity of molecules using machine learning techniques with Merck's provided dataset that includes molecular descriptors and biological activity using Quantitative structure-activity relationships (QSAR) prediction. The dataset is preprocessed to make it suitable for modeling by handling missing values, converting categorical variables, and feature scaling. Visualization techniques are used to explore the data and identify relationships between features and biological activity. Various machine learning algorithms are employed to create models that predict biological activity, which are then evaluated using performance metrics. The most important features contributing to the prediction of biological activity are identified using feature importance plots created by the Random Forest model.

# Objective & Data
The objective of this Merck data challenge is to identify the best statistical techniques for predicting biological activities of compounds against specific molecules given the numerical descriptors generated from the chemical structures of these compounds.
The data provided by Merck is based on 15 target molecules and over 20,000 compounds for each target. For each target molecule, each row of the data corresponds to a compound and contains descriptors derived from that compound's chemical structure. Activity between the target molecule and each compound is provided in the training data and is the target for prediction in the test data.

# Evaluation Metric
Predictions for activity will be evaluated using the correlation coefficient R2, averaged over the 15 data sets. For each data set,

![image](https://user-images.githubusercontent.com/25953950/222567550-681b4429-3f5a-42e0-a877-5ce9daf4b15d.png)

where x is the known activity, x¯ is the mean of the known activity, y is the predicted activity, y¯ is the mean of the predicted activity, and Ns is the number of molecules in data set s. An R2 of 1 indicates the predictions perfectly fit the data.
