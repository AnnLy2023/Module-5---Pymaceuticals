# Module-5---Pymaceuticals

Background
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.
As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

Tasks:


Step 1. Prepare the data.
Prepare the Data
Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.
Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.
Display the updated number of unique mice IDs.
![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/eded9e84-70c9-435a-a473-ce7fead75622)
![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/12a59a93-6420-4a03-a5c8-21badb2f1b8f)
![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/e7e7deae-5f6d-45cd-bc39-11ee04863421)



Step 2. Generate summary statistics.
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.
Your summary statistics should include:
  -A row for each drug regimen. These regimen names should be contained in the index column.
  -A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

  
![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/3c42cfc4-f929-40de-9847-1f00aff8e7ce)


3. Create bar charts and pie charts.
Create Bar Charts and Pie Charts
Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.
Create the first bar chart with the Pandas DataFrame.plot() method.
Create the second bar chart with Matplotlib's pyplot methods.
Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.
Create the first pie chart with the Pandas DataFrame.plot() method.
Create the second pie chart with Matplotlib's pyplot methods.
Bar charts

Pandas Df.plot () method

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/270569ac-b622-4a44-b8d6-9df88d5eea88)



Matplotlib's pyplot method


![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/7db778a6-b985-4ef3-bc80-cd6507e62ff8)


Pie Charts

Pandas DF.plot() method

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/81625f27-b779-4e39-8899-6ddf6fd58330)


Matplotlib's pyplot method

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/f053ecc6-b17e-47e2-a3c2-277d964ff074)



4. Calculate Quartiles, Find Outliers, and Create a Box Plot
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:
Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/1a163bad-e51c-4b23-84a7-6a610bfcf6e4)

Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
Determine outliers by using the upper and lower bounds, and then print the results.

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/6061d5af-f7e3-4d75-8ed8-8754c93e414e)

Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/f6e509f7-b5f2-4ce2-b866-8d3f69e3c3d2)


Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/5d2c2670-1372-4add-b6af-d21911e5740a)



Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/71132abe-00cc-4187-b763-0c8ca6b1d283)


5. Calculate Correlation and Regression
Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.

![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/8c1126b0-7069-4c77-9591-a2b30d6b9865)

Plot the linear regression model on top of the previous scatter plot.
![image](https://github.com/AnnLy2023/Module-5---Pymaceuticals/assets/129100456/5d689ae1-21ac-4d69-aefe-7d3c49e70fbc)








