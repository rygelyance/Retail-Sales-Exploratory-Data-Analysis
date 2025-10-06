# Retail Sales Exploratory Data Analysis

THIS PROJECT IS CURRENTLY IN PROGRESS

## Introduction
This is a project designed to demonstrate my skills in exploratory data analysis to deliver key visualizations and actionable insights through a Power BI dashboard.

## The Dataset
The dataset I used is the "Superstore Sales" dataset from [Kaggle][https://www.kaggle.com/datasets/ishanshrivastava28/superstore-sales]. This dataset contains 
a diverse set of daily information across a four-year period on product sales, including sale locations, product descriptions and categories, and order and shipping dates, among others.

## Data Structuring and Cleaning
Most of the work done prior to analysis of this data was to split the original data into a fact table and several dimension tables in a Star Schema. In Power BI, this helps the performance of visuals and enable better filtering, grouping, and summarization. Below is the schema I created from the original table:
![image](Images/StarSchema.png)
However, outside of this, there were some minor modifications and data cleaning to be performed. For example, I needed to utilize a Change Type using Locale step to convert the Order Date and Ship Date to the proper type, as they were in the format dd-mm-yyyy, which Power Query was unable to automatically parse.