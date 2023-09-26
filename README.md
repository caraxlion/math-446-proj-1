# math-446-proj-1
Assignment-1 for Mathematics 446 - Data Science in Python

Goal: Using the new scores.csv dataset, determine the course letter grade of each student.
The evaluation standards in the course are the following:

i. Only students having taken at least two midterms and the final exam can be assigned
a course letter grade.

ii. For students who missed a midterm but took the final exam, their missing midterm
scores should be inferred using a linear regression ”missing midterm” against quiz
ave once quiz ave for each student has been calculated.

iii. Grading breakdown: Quiz ave, 15%; Midterm ave, 45%; Final 40%.

iv. For each student, Quiz ave should be calculated dropping the lowest two scores.

v. For each student, Midterm ave should be calculated as a weighted ave: highest score,
45%; 2nd best score, 35%; lowest score, 20%.

vi. After aggregating the dataset to obtain Quiz ave, Midterm ave, and Final score for
each student, a letter grade should be assigned for each of 3 performances. Assignment
of the letter grade for each performance should be done using the pd.cut function. You
are the one determining the cut-offs. However, your methods to calculate the cut-offs
should be clearly explained and justified based on exploratory data analysis (statistical
analysis, data visualization, etc.).

vii. There are 12 letter grades: A, A−, B+, B, B−, C+, C, C− , D+, D, D−, F. The GPA
scores associated with these letter grades are 4, 3.7, 3.3, 3, 2.7, 2.3, 2, 1.7, 1.3, 1, 0.7,
0, respectively.

viii. Once the GPA course weighted ave is calculated for each student, the pd.cut function
should be used to determine the course letter grades with the following cut-offs: 
4,3.85, 3.55, 3.15, 2.85, 2.55, 2.15, 1.85, 1.55, 1.15, 0.85, 0.55, 0.

ix. Your final aggregated data frame should display:
• GPA score for Quiz ave;
• GPA score for Midterm ave;
• GPA score for Final;
• GPA course weighted ave;
• Course letter grade.

Your dataset should be sorted by GPA course weighted ave in decreasing order.

Your submission must be a Markdown ipnb report, well-structured and organized. It must
include the code, comments explaining your methods and reasoning, the relevant outputs,
etc. You will submit both a printed version of your report and the ipnb file. Max total
of pages is 10, default front-size. Your report must be printed one-sided, with two pages
side-by-side.
