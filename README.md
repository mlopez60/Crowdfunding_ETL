# Crowdfunding_ETL

### Project 2
### Team Members: Matthew Lopez, Mitchell Fairgrieve and Steven Carrasquillo

For the ETL mini project, you will work with a partner to practice building an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions to extract and transform the data. After you transform the data, you'll create four CSV files and use the CSV file data to create an ERD and a table schema. Finally, you’ll upload the CSV file data into a Postgres database.

Since this is a one-week project, make sure that you have done at least half of your project before the third day of class to stay on track.

Although you and your partner will divide the work, it’s essential to collaborate and communicate while working on different parts of the project. Be sure to check in with your partner regularly and offer support.

### Process
1. Create the Category and Subcategory DataFrames
    1. Extracted and transformed the crowdfunding.xlsx Excel data to split the 'category & subcategory' column
    2. Created a DataFrame for the category and added category_id field
    3. Did the same for the subcategory
    4. Exported both DataFrames into csv files

2. Create the Campaign DataFrame
    1. Extract and transform the crowdfunding.xlsx Excel data to create a campaign DataFrame
    2. Renamed some columns
    3. Converted 'goal' and 'pledged' columns to float format
    4. Converted 'launch_date' and 'end_date' columns to datetime format
    5. Exported DataFrame to campaign_csv file

3. Create the Contacts DataFrame (selected Option 1: Use Python dictionary methods)
    1. Imported the contacts.xlsx file into a DataFrame.
    2. Iterated through the DataFrame, converting each row to a dictionary.
    3. Iterated through each dictionary extracting the dict. values from the keys by using list comprehension.
    4. Created a new DataFrame that contains the extracted data.
    5. Split each "name" column value into a first and last name, and place each in a new column.
    6. Cleaned and exported the DataFrame as .csv file

4. Create the Crowdfunding Database
    1. Created an ERD sketch based on the 4 created csv files using QuickDBD
    2. Using the ERD, created a database schema
    3. Created a new Postgres database and used the database schema to create tables for the data
    4. Imported each csv file to their respective tables
    5. Ran queries for each table to verify the data and table was correct
