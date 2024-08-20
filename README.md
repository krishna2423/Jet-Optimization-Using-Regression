# Jet optimization using a linear regression model and statistical methods in dimuon collisions 

# This program uses the 2010 and 2011 CERN dimuon collision datasets in order to make predictions on the noise of dimuon collisions using features such as the mass and transverse momentum

#Regression Model
This project starts with data preprocessing and cleaning using data visualization and other preprocessing methods in python (with libraries such as pandas, numpy, matplotlib, and seaborn). With the revised dataframe, feature engineering takes place to  find the right features to input into the model. Instead of using a more classice data science approach such as KBest or embedded models, this program uses domain knowledge of the features to create a new one which when paired with the noise and initial energies, creates a very high accuracy when fed to the regression model. This works to confirm the relationship between noise found in this paper: https://emerginginvestigators.org/articles/23-180 

#Math Computations
To find the experimental ranges of our dataset, we used mathematical Python functions as well as the noise equation we derived using methods mentioned in materials and methods section to find the ideal ranges that would minimize the noise as in the top quartile of our data. For our initial parameters, we used the median values of each variable within the top quartile and selected the noise to be the median of the top quartile of noise values. We then solved for each target variable, concerning the other assumed
values. We then worked backwards to find the ideal ranges for the rest of the input parameters. 
