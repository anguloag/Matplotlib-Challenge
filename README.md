# Pymaceuticals: Matplotlib Challenge
### Objective
Develop a code using python, pandas, and matplotlib to analyze the results of Pymaceuticals' recent animal study of potential treatments for squamous cell carcinoma, and develop summary tables and figures that compare the performance of Pymaceuticals' Capomulin to other treatment regimens. 

### Description of the Data: Mouse_metadata and Study_results
The metadata for all 249 mice included in the study are contained in a csv file called "Mouse_metadata". The dataset is organized into five columns: 
- Mouse ID - the unique ID number for each mouse 
- Drug Regimen - the drug treatment assigned to each mouse (Capomulin, Placebo, or one of 8 other drug regimens)
- Sex - the sex of each mouse (Male or Female)
- Age_months - the age of each mouse, measured in months
- Weight (g) - The weight of each mouse, measured in grams 

The data for the results of the drug trials are contained in a csv file called "Study_results". The dataset is organized into four columns:
- Mouse ID - the unique ID number for each mouse 
- Timepoint - the timepoint in which the data was taken (0, 5, 10, 15, 20, 25, 30, 35, 40, and 45). Going down the rows, the data is organized chronologically such that all of the results from each timepoint are grouped together going from time 0 to time 45. 
- Tumor Volume (mm3) - the tumor volume for each mouse, measured at each timepoint in cubic millimeters 
- Metastatic Sites - the number of metastative sites for each mouse at each timepoint

### What the Code Should Do
The code should merge the data from Mouse_metadata and Study_results into one dataset, and should create the following summary tables (titled and labeled appropriately):
- A Summary Statistics Table, which includes the mean, median, variance, standard deviation, and standard error from the mean (SEM) of the tumor volume for each drug treatment 
- Bar Plots that show the total number of timepoints for all mice tested for each drug treatment throughout the course of the study, generated using Pandas DataFrame.plot() and Matplotlib's pyplot
- Pie Charts the show the percentage of male and female mice included in the study, generated using Pandas DataFrame.plot() and Matplotlib's pyplot
- A Box and Whisker Plot of the final tumor volumes for the four most promising treatment regimens, which highlights potential outliers by changing their color and style in the plot (generated with Matplotlib)
- A Line Plot of tumor volume versus time point for one mouse treated with Capomulin
- A Scatter Plot of tumor volume versus mouse weight for the mice treated with Capamulin, with the linear regression model printed on the plot

Finally, at least three observations based on the generated charts and tables should be listed at the top of the code notebook. 
