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
    - Decision Trees and Random Forests SKT.ipynb
        
        Creating a random forest model
    - kNN and average Models-SKT.ipynb
        
        Creating a k Nearest Neighbors model, as well as models where only one feature was taken and the prediction was determined by which side of "average: of that feature the observation was on.
    - Logistic Regression SKT.ipynb 
    
        Creating a logistic regression model using all of the features, as well as making one for each feature individually
    - Support Vector Classifier.ipynb
    
        Creating a SVC model using all of the features, where the classification data was target encoded
    - TE-Decision Trees and Random Forests SKT.ipynb
    
        Repeating 'Decision Trees and Random Forests SKT.ipynb' where the classification data was target encoded
    - TE-kNN and average Models-SKT.ipynb
    
        Repeating `kNN and average Models-SKT.ipynb` where the classification data was target encoded
    - TE-Logistic Regression SKT.ipynb
        
        Repeating `Logistic Regression SKT.ipynb` where the classification data was target encoded
    - Voting Models.ipynb
    
        Creating a voting model using the 4 best models created so far.


        
