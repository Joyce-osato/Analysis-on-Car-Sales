# CAR SALES EXPLORATORY DATA ANALYSIS WITH PYTHON

## Introduction
The analysis done was to compare and correlate manufacturers of cars and other variables that would determine the rate of purchase and the choice of brand to purchase.
The analysis seeks to proffer inference to why some brands are more purchased than others and some factors that would influence the purchase of those products.
The analysis was done using the PYTHON PROGRAMMING LANGUAGE and the jupyter notebook

## Data Sourcing
The dataset was sent to an email from the facilitator Mr Joseph Elijah, the email contains two files; which was the dataset and the other was questions and guide used in analyzing and answering the questions relating to the dataset.

## Data Preprocessing
The code for importing data libraries and file was imputed to prepare the python workspace
Numpy is imputed to work with numbers/integers, Pandas; to work on Series or Dataframe and also to alter data, Matplotlib and Seaborn are used for data visualization
The file was saved in a csv format and was uploaded as such.
And the dataset was displayed as shown below;
 
![image](https://github.com/user-attachments/assets/b299c112-a2d6-4b42-aaec-f7b3294b2bb4)



## DATA EXPLORATION
1.	 How many rows and columns are present in the dataset?

![image](https://github.com/user-attachments/assets/538cbaea-32c0-41e9-a94b-5ff77c1dc94a)

There are 157 rows and 16 columns from the dataset presented above

2. What are the data types of each column? Are the data types for each column
appropriate? If not change the data types of some columns to what they are
supposed to be
Using the “data.dtypes” code, all columns with string values are classified as ‘objects’ and columns with decimals or integers are classified as ‘float’ data types.
 
![image](https://github.com/user-attachments/assets/9c768f11-271e-4682-a53c-db2a80b63505)

## DATA CLEANING
3. Are there any missing values in the dataset? If so, how many and in which
columns? Fill the missing values in the year_resale_value with the average
year_resale_value, then drop all other rows with missing values in the dataset

![image](https://github.com/user-attachments/assets/856d33ec-c77e-4328-8638-cd1ba39fd17b)

Data was cleaned by checking for and counting missing values using the data.isna().sum() and these were replaced by finding the average of the column affected and replacing the null values with them, afterwhich all other rows with missing values were dropped using the data.dropna()

![image](https://github.com/user-attachments/assets/137c1590-4599-47aa-b9f3-4264af7a10ef)

4. Clean the name of the __year_resale_value column by removing the leading
underscore 

 ![image](https://github.com/user-attachments/assets/98905a2e-7d73-467b-be83-00f9df6bd72b)



6. Check if the dataset has any duplicates. If there are, drop them
 
![image](https://github.com/user-attachments/assets/32f5c3d3-b86b-428e-9dab-f4a196714845)


## DESCRIPTIVE STATISTICS
5. Do descriptive statistics (mean, median, standard deviation) of
the numerical columns. What do you notice?


 

EXPLORATORY DATA ANALYSIS
6. Which manufacturer has the highest and lowest average sales volume?
The ‘Manufacturer’ and ‘Sales_in_thousands’ are grouped using the function group_by and the mean is also imputed and idmax()/idmin() is used to determine the highest and lowest sales volume 
 
 ![image](https://github.com/user-attachments/assets/c2106d9b-aa45-4e57-ac92-da0f2900b9b9)
![image](https://github.com/user-attachments/assets/9cdb7ca4-c59d-4b42-ac9b-f532c5745617)






7. What is the distribution of car prices in the dataset?

 ![image](https://github.com/user-attachments/assets/69d1d2a4-6e74-47f7-901e-be475133663a)

 
![image](https://github.com/user-attachments/assets/1e46bf01-0851-44f9-b411-68e82c2d32b2)


8. Plot a correlation matrix to see if different numerical variables in the dataset
correlate with each other.
Before plotting the matrix, a code to first create the correlation is imputed

 ![image](https://github.com/user-attachments/assets/65575cdd-57d5-4d4f-ace2-f77dd15c1eaf)

Then the matrix is plotted
 ![image](https://github.com/user-attachments/assets/a4993bbc-07c9-4a63-be01-953d2b7fea45)


9. Plot the relationship between price and latest launch year.

![image](https://github.com/user-attachments/assets/13cd923a-6dae-453f-abd3-fba3bcf566e1)

![image](https://github.com/user-attachments/assets/42760aa8-8ba3-431b-842e-c0cb0d2e531f)

To plot the relationship between price and launch year, the data type of latest launch had to be changed first
 
 ![image](https://github.com/user-attachments/assets/cc8bdc80-ebb0-4a53-9812-695ac793d565)

 

10. Group cars by manufacturers and analyze their average price and fuel
efficiency.
 
![image](https://github.com/user-attachments/assets/169de1f6-3162-47e4-9cdb-52fde0fc3fc3)

11. Can you identify and visualize the most popular car brands?
 ![image](https://github.com/user-attachments/assets/4e4bb392-1981-4c08-a9d5-c132d4f4012f)

 
From the analysis, the F-series from the Ford company is the most popular car brand

12. Which car model has the highest resale value compared to its initial price?
 ![image](https://github.com/user-attachments/assets/ec924ba7-364a-4ab9-9690-40c42b3994a3)


13. Find the top 3 fuel-efficient cars with an engine size above 2.5 liters.

 ![image](https://github.com/user-attachments/assets/c9fe59c8-378e-4542-aec6-e449dbe7281f)

The top 3 fuel-efficient cars with engine above 2.5 litres are Chevrolet Impala, Chevrolet Monte Carlo and Mercedes-B CLK Coupe

14. Which Lexus model has the highest horsepower?
 ![image](https://github.com/user-attachments/assets/ec71c56b-e1e1-4067-9426-22df6301dc60)

