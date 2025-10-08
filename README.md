# Retail Sales Exploratory Data Analysis

THIS PROJECT IS CURRENTLY IN PROGRESS

## Introduction
This is a project designed to demonstrate my skills in exploratory data analysis to deliver key visualizations and actionable insights through a Power BI dashboard.

## The Dataset
The dataset I used is the "Superstore Sales" dataset from [Kaggle][https://www.kaggle.com/datasets/ishanshrivastava28/superstore-sales]. This dataset contains 
a diverse set of daily information across a four-year period (2011-2014) on product sales, including sale locations, product descriptions and categories, and order and shipping dates, among others.

## Data Structuring and Cleaning
Most of the work done prior to analysis of this data was to split the original data into a fact table and several dimension tables in a Star Schema. In Power BI, this helps the performance of visuals and enable better filtering, grouping, and summarization. Below is the schema I created from the original table:
![image](Images/StarSchema.png)
However, outside of this, there were some minor modifications and data cleaning to be performed. For example, I needed to utilize a Change Type using Locale step to convert the Order Date and Ship Date to the proper type, as they were in the format dd-mm-yyyy, which Power Query was unable to automatically parse.

## Dashboard Visuals & Initial Insights
The main dashboard is displayed in the image below and was the bulk of the work for this project, leveraging my skills within Power BI and the DAX language.
*Final image to be added*

### Cards
I added three main cards underneath the title displaying three key metrics, the total sales for the selected periods, the total profit, and the total quantity of sales. There isn't too much interesting from this, but it can be seen through these cards and selecting the years that the total profits and total quantity of sales have consistently gone up year-over-year. Interestingly, the total sales figure went down between 2011 and 2012, but profits still increased.

### Slicers
I opted to add four slicers in total, selecting the year, quarter, segment (Consumer, Corporate, and Home Office), and the state the sale was made in.

### Total Profit by State
From this data, sales were made across 42 states in total (including the District of Columbia as one). While most states were profitable, with the most profit being produced in California and New York, there were a number of states that consistently produced a net loss on profit, with Texas sales consistently having the largest losses. Further investigation into sales in these states would be a good idea for this store, and that analysis is something I dive further into in the following section.

### Total Quantity by Category
This visual represents the distribution of categories that the company sells, with the vast majority of the company's sales being in the category of office supplies.

### Highest and Lowest Profit Products
These visuals allow a business to immediately see which products are producing the most profit for the company and which are producing the heaviest losses. This could allow the company to negotiate better deals with the manufacturers of the least profitable products or to cut those products from their lineup. Over a longer time period than this dataset, these visuals could also allow a company to see emerging trends or shifts (i.e. the top 5 profitable products might all be phones in the latest year).

### Total Profit by Month
This allows for analysis of the most profitable times throughout each year of data, and across all years, the end of the year is consistently the most profitable time for this superstore, with Quarter 4 having the highest average profit of $36,910.44 and the month of December having the highest average profit of all months at $43,436.13. In addition, I've applied conditional formatting to this visual to indicate which months perform above or below the average and any months that produced a net loss in profit.

### Total Profit by Sub-Category
This gives a breakdown of profits gained or lost by each sub-category of product. For this superstore, the products that produce the most profit are Copiers, Phones, and Accessories, while Tables produce the largest net loss.

## Key Insights & Recommendations
*In Progress*