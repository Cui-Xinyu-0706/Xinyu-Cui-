Data Visualization Exercises
This repository contains solutions for six data visualization exercises using Python with Pandas, Seaborn, and Matplotlib libraries. The exercises analyze a dataset containing student information, including their study habits, grades, and course enrollments. Below is a detailed explanation of each task.

Dataset Description
The dataset used for these exercises includes the following columns:

Student Name: Name of the student.
Course: The course in which the student is enrolled.
Grade: The student's grade in the course (out of 100).
Gender: The gender of the student.
Study Time: The number of hours the student spends studying.
Age: The student's age.
Exercises
1. Lineplot: Study Time by Student Name
Objective: Display how each student's study time varies.
Visualization: A lineplot with "Student Name" on the x-axis and "Study Time" on the y-axis.
Result: Identified Edgar as the student with the highest study time.
2. Histogram: Grade Distribution
Objective: Plot the frequency distribution of grades.
Visualization: A histogram with bins showing the count of grades.
Result: The grade range 85 to 90 had the highest frequency of students.
3. ECDF Plot: Percentage of Students Scoring Less than 85
Objective: Create an ECDF (Empirical Cumulative Distribution Function) plot for grades and compute the percentage of students scoring below 85.
Visualization: A cumulative distribution curve.
Result: Approximately 28.57% of students scored less than 85.
4. Stripplot: Grade Distribution by Course
Objective: Visualize the distribution of grades for each course.
Visualization: A stripplot with jittered points to represent individual grades for each course.
Result: Cloud Computing had the most spread in grades.
5. Swarmplot: Study Time by Gender
Objective: Show the relationship between gender and study time.
Visualization: A swarmplot where dots represent individual students' study times grouped by gender.
Result: Female students had a higher average study time than males.
6. Pointplot: Average Grade by Course
Objective: Display the average grade for each course.
Visualization: A pointplot with markers showing the mean grade for each course.
Result: Computer Vision had the highest average grade.
Libraries Used
Pandas: Data manipulation and analysis.
Seaborn: Statistical data visualization.
Matplotlib: Base library for creating static, animated, and interactive visualizations.
How to Run
Clone the repository.
Install the required libraries:
bash
pip install pandas matplotlib seaborn
Run the script file visualization_exercises.py or use Jupyter Notebook to visualize the plots.
Insights and Observations
The visualizations provide valuable insights:

Students in Computer Vision generally perform better, as shown by the highest average grade.
Cloud Computing shows variability in grades, indicating differing levels of student performance.
Female students, on average, study more than male students, as observed in the swarmplot.

