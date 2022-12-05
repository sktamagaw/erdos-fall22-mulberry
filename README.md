# erdos-fall22-mulberry
<h2>Code for Erdos Data Science Bootcamp Fall 2022 </h2>

This repository contains Python code for the Erdos Data Science Bootcamp Fall 2022.

<ul>
    <li> Data 
        <p> This folder contains the data we used to build our model, as well as the Jupyter notebooks we used to clean and explore the data.</p>
        <ul>
              <li> Data Cleaning-SKT.ipynb </li>
  
  A short file where I made the data easily usable in Pandas
  
  <li> Data Cleaning 2-SKT.ipynb </li>
  
  A file where I adjusted some of the parameters to make more sense, and added columns that were found to be useful in `Exploratory Data Analysis-SKT.ipynb`
  
  <li> Data Cleaning 3-Target Encoding SKT.ipynb </li>
  
  A file where I added target encoded columns for the categorical features pay history, sex, education, marriage, age, and age grouped by 10's
  
  <li> Exploratory Data Analysis-SKT.ipynb </li>
  
  Looking at the different features of the data to see which ones seemed helpful, and adding a few new features based on them
        </ul>
    </li>
    
    
    <li> Models </li>
    
    </ul>


Python Files:
<ul>

  
  <li> kNN and average Models-SKT.ipynb </li>
  
  Creating a k Nearest Neighbors model, as well as models where only one feature was taken and the prediction was determined by which side of "average: of that feature the observation was on.
  
  <li> Decision Trees and Random Forests SKT.ipynb </li>
  
  Creating a random forest model
  
  <li> Logistic Regression SKT.ipynb </li>
  
  Creating a logistic regression model using all of the features, as well as making one for each feature individually
  
  </ul>


Other files:
<ul>
    <li>clean_data_2.csv </li>
  
  The CSV file created in `Data Cleaning 2-SKT.ipynb`
  
  <li> clean_data_3.csv </li>
  
  The CSV file created in `Data Cleaning 3-SKT.ipynb`

  <li>dataset_2_description.txt </li>
  
  A description of what every column in `clean_data_2.csv` represents
  
  <li> dataset_3_description.txt </li>
  
</ul>
