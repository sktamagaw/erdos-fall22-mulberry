#### erdos-fall22-mulberry

# Code for Erdos Data Science Bootcamp Fall 2022 

This repository contains Python code for the Erdos Data Science Bootcamp Fall 2022.

- Data

    This folder contains the data we used to build our model, as well as the Jupyter notebooks we used to clean and explore the data.
    - Data Cleaning-SKT.ipynb
    
        A short file where I made the data easily usable in Pandas
    
    - Data Cleaning 2-SKT.ipynb
        
         A file where I adjusted some of the parameters to make more sense, and added columns that were found to be useful in `Exploratory Data Analysis-SKT.ipynb` 
    - Data Cleaning 3-Target Encoding SKT.ipynb 
    
        A file where I added target encoded columns for the categorical features pay history, sex, education, marriage, age, and age grouped by 10's
    - Exploratory Data Analysis-SKT.ipynb
    
        Looking at the different features of the data to see which ones seemed helpful, and adding a few new features based on them. A summary of the findings can be found [here](https://docs.google.com/document/d/1MDKqtuiMJgI825MwL7AHRbN92E5kdDWzO5WiqwCGklg/edit)    
    - clean_data_2.csv
        
        The CSV file created in `Data Cleaning 2-SKT.ipynb`
    - clean_data_3.csv 
        
        The CSV file created in `Data Cleaning 3-SKT.ipynb`
    - dataset_2_description.txt
        
        A description of what every column in `clean_data_2.csv` represents
    - dataset_3_description.txt
    
        A description of what every column in `clean_data_3.csv` represents
     
- Models
    
    In this folder contains the various models we fit to our data.  A summary of the models as well as their metrics (accuracy and recall) can be found [here](https://docs.google.com/document/d/1pvSNpeU0y08Zb_ih3pMUEUaLIaNn1fhClf9ShCIiy38/edit#)
    
    - Baseline.ipynb
    
        Creating a baseline using random guessing with various probabilities, and comparing our best models against it.  We can plainly see that if recall is important to us and we're willing to lose a little accuracy, the k Nearest Neighbors model is the best.  Otherwise, the voting model performs the best overall.
    
    - Decision Trees and Random Forests SKT.ipynb
        
        Creating a random forest model.  We see that max_depth levels off after about 6, and n_estimators doesn't seem to vary the results much, so we might as well use 2.
    - kNN and average Models-SKT.ipynb
        
        Creating a k Nearest Neighbors model, as well as models where only one feature was taken and the prediction was determined by which side of "average" of that feature the observation was on.  The models in this notebook generally have bad accuracy or recall.
    - Logistic Regression SKT.ipynb 
    
        Creating a logistic regression model using all of the features, as well as making one for each feature individually.  On the individual features, we notice that only the most recent payment history, average pay history, and total number of unpaid months were the only models that didn't just assume no one defaulted.  So, we also created a model that used only these three features, and that performed better.  Varying C didn't matter much.
        
    - Neural Network Models.ipynb
    
        Creating Neural Network Models.  A summary of these can be found [here](https://docs.google.com/document/d/1RBTwPmg-FhYvKPpLcc3vhlfQJsN615UCrALc_UfR7oo/edit)
    - Support Vector Classifier.ipynb
    
        Creating a SVC model using all of the features, where the classification data was target encoded.  We found that among polynomials with degree up to 15, linear, rbf, and sigmoid, the sigmoid kernel performed the worst, and the others performed about that same.  We also found that only using the features used on the logistic regression model also performed slightly better.
    - TE-Decision Trees and Random Forests SKT.ipynb
    
        Repeating 'Decision Trees and Random Forests SKT.ipynb' where the classification data was target encoded.  We had similar results to before, though the models perfomed slightly better.
    - TE-kNN and average Models-SKT.ipynb
    
        Repeating `kNN and average Models-SKT.ipynb` where the classification data was target encoded.  We also remembered to scale the data and apply PCA first.  We found that using an odd number of neighbors seemed to work better, and the optimal number of neighbors to use was 3.
    - TE-Logistic Regression SKT.ipynb
        
        Repeating `Logistic Regression SKT.ipynb` where the classification data was target encoded.  We had similar results to before, though the models performed slightly better.
    - Voting Models.ipynb
    
        Creating a voting model using the 4 best models created so far.  The best voting model occured when using only a few features to train the Logistic Regression and SVC models, using the other features on the Random Forest and k Nearest Neighbor model, and breaking ties by assuming 1.


        
