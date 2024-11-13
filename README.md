 Data Handling and Transformation Exercises

Overview
This project includes exercises on data handling and transformation using pandas, focusing on tasks such as creating new columns, joining DataFrames, and extracting string data. Each exercise aims to enhance skills in handling missing data, transforming data, and performing basic data manipulation.

Table of Contents
1. [Exercise 1: Creating Initials Column](#exercise-1-creating-initials-column)
2. [Exercise 2: Joining DataFrames](#exercise-2-joining-dataframes)
3. [Exercise 3: Combining DataFrames](#exercise-3-combining-dataframes)
4. [Exercise 4: Extracting Last Names](#exercise-4-extracting-last-names)
5. [Setup and Requirements](#setup-and-requirements)
6. [Usage](#usage)
7. [Results](#results)

 Exercise 1: Creating Initials Column
Objective: Create a new column called `professor_initials` that stores the initials of each professor's first and last names.
Solution: Using string operations, split the professor's name and extract the initials of the first and last names.
Exercise 2: Joining DataFrames
Objective: Use join to combine the original df DataFrame with a new df_courses DataFrame on the professor column.
courses_data = {
    'professor': ['Ludmila Kuncheva', 'Antonio Torralba', 'Manuel Gonzalez', 'Bastian Leibe'],
    'courses': ['Machine Learning', 'Computer Vision', 'AI Programming', 'Self-Driving Cars']
}
Solution: Use the join function to merge df with df_courses based on the professor column, creating a new combined DataFrame.
Exercise 3: Combining DataFrames
Objective: Combine the original df and df_courses DataFrames to form a single DataFrame with all information.
Solution: Use either merge or concat to combine the data from both DataFrames into a single DataFrame.
Exercise 4: Extracting Last Names
Objective: Create a new column called professor_last_name by extracting the last name of each professor using string operations.
Solution: Apply string splitting to extract the last name from the professor column and store it in a new column called professor_last_name.
