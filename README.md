# FIFA 20 Player Analysis Project
 
 # Tableaue Visualization: 
 ![](https://github.com/mdrhmn48/Fifa20Game-dataset/blob/main/Screenshot_20230724_045631.png)

# link: https://public.tableau.com/app/profile/md.rahman5916/viz/FFIA20/Dashboard2

This project is focused on analyzing and visualizing data related to FIFA 20 players using Python and various libraries, including Pandas, Matplotlib, Seaborn, and Boto3. The goal is to extract insights from the dataset and create visualizations to understand player attributes and distributions.
Requirements

Before running the code, make sure you have the required dependencies installed:

    boto3 (!pip install boto3)
    pandas (import pandas as pd)
    os (import os)
    logging (import logging)
    matplotlib (import matplotlib.pyplot as plt)
    seaborn (import seaborn as sns)
    KEYS.py - Ensure you have a file named KEYS.py containing your AWS access key and secret access key as variables ACCESS_KEY and SECRET_ACCESS_KEY.

# Functionality
1. Uploading and Downloading Files from Amazon S3

The project uses the Boto3 library to interact with Amazon S3. The upload_file and download_file functions allow you to upload a local file to an S3 bucket and download a file from S3.
2. Data Loading and Exploration

The project loads the FIFA 20 player data from a CSV file named "players_20.csv" into a pandas DataFrame. It then performs various exploratory data analysis tasks:

    Display the top 5 records from the dataset.
    Show the names of all columns in the DataFrame.
    Display the number of rows and columns in the dataset.

3. Country-wise Player Count

The project calculates the number of players from each country and presents the result in a pandas DataFrame.
4. Top 10 Countries with the Most Players

The project filters and presents the top 10 countries with the highest number of players.
5. Bar Plot of Top 5 Countries and Their Player Count

The project creates a bar plot to visualize the top 5 countries with the highest number of players, filled with the color green.
6. Top 5 Players with Highest Wages

The project identifies and displays the top 5 players with the highest wages.
7. Top 5 Players with Highest Salaries

The project identifies and displays the top 5 players with the highest salaries, including both wages and value.
8. Bar Plot of Top 5 Players with Highest Salaries

The project creates a bar plot to visualize the top 5 players with the highest salaries.
9. Analysis of Germany Players

The project filters the dataset to show the top 10 players from Germany based on different attributes like overall, height, weight, and wages.
10. Analysis of USA Players

The project converts the value from Euros to USD and identifies the top 5 players from the United States based on their value in USD.
11. Data Visualizations

The project includes several data visualizations, such as a scatter plot of overall rating vs. wage, bar plots of average value USD vs. age and average wage EUR vs. team position, and a pie chart showing the top 10 clubs by spending.
12. Saving and Uploading the Updated Data

The project saves the updated DataFrame to a new CSV file named "players20_updated.csv" and then uploads it to the specified S3 bucket.
