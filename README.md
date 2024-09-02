# National Stock Number (NSN) Data Analysis Project
## Project Overview
This project involves an in-depth analysis of National Stock Number (NSN) data, with a focus on exploring pricing patterns across various representative offices. The primary objective is to determine whether there are significant differences in average prices among different representative offices and to identify factors contributing to these differences.

The project includes a comprehensive analysis process, including exploratory data analysis, hypothesis testing, predictive modeling, and the development of a Shiny application for interactive data exploration.

## Data
The dataset used in this project contains the following key variables:

NSN: The National Stock Number identifying each item.
RepOffice: The representative office responsible for the item.
Common Name: A general name or description of the item.
Description: A detailed description of the item.
Price: The price of the item.
Dataset Summary
Rows: 12,454
Columns: 7 (after cleaning and processing)

## Data Cleaning
The cleaning process involved:

Handling missing values
Ensuring that the Price column was numeric
Converting appropriate variables to factor data types

## Analysis Process
1. Exploratory Data Analysis (EDA)
Summary statistics for the Price variable, revealing a right-skewed distribution.
Pricing analysis by representative office, showing variations in average prices.
Text analytics on product descriptions to identify key product features.
2. Hypothesis Testing
ANOVA was conducted to test the hypothesis that average prices differ across representative offices.
Assumptions of normality and homogeneity of variances were checked before the test.
3. Predictive Modeling
PCA & Regression Analysis: PCA was performed to reduce dimensionality, followed by a regression analysis.
Random Forest: A Random Forest model was applied to improve predictive performance.
4. Shiny Application
An interactive Shiny application was developed to explore the data and analysis results in real-time.
![image](https://github.com/user-attachments/assets/0abe3902-0099-4a2a-bfec-288f5d325306)

## Running the Application
To run the Shiny application:

Ensure you have all the required libraries installed:

install.packages(c("shiny", "shinydashboard", "ggplot2", "dplyr", "tm", "wordcloud", "forecast", "DT", "randomForest"))
Run the application using the following R script:

shinyApp(ui = ui, server = server)

## Conclusion
The analysis revealed significant differences in average prices across different representative offices, likely due to variations in product types or pricing strategies. The Shiny application provides an interactive platform for stakeholders to explore the data further and make informed decisions.
