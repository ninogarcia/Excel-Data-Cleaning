# Excel-Data-Cleaning
## Data Cleaning and Preparation

Scenario: You have received some sales data from your company's database. The data is in a dirty format and you are required to clean it up in order to perform some analysis on it. Since your company will need to perform this analysis each month with new data, you are to use formulas to clean the data so that the workbook can be easily updated each month with new records from the database. Follow the instructions carefully and answer the questions as you go.	

### Question 1
Look at the Data worksheet and Clean worksheet. Make sure the Check Sum value in Data cell B2 is 95858 (90898 on Excel for Mac 2011). Do not insert any rows or columns into the Data sheet during your work or the Check Sums may give different results than programmed.

Our goal is to populate the columns of the Clean worksheet with the data in a form that we can easily analyse. This may look daunting, but we are told by the Data Manager that the raw data always follows a certain pattern. That pattern is:

1. Some / characters

2. The product type sold, with the prefix PR:

3. Some "_" characters

4. The Sales Person's name, with the prefix SP:

5. The date of the sales, in the format yyyymmd. All sales are from October 2017

6. Some non-breaking space characters

7. The amount of sales, with the prefix $. All sales amounts are below $10000

8. Some space characters

9. A final random character that has an ASCII value between 28 and 31.

We will clean up the data one item at a time, by using formulas to make copies of the data to the right of column B, with each copy being slightly cleaner than the previous. When we are done we will separate the data into 4 components on the Clean worksheet tab, and perform some basic analysis.

Go to the Data worksheet. To begin, we want to verify what special characters might be at the end of each data entry. In column C (cells C5:C500) write a formula using the RIGHT and CODE functions to return the ASCII code of the final character in each record.

How many records have the character 30 as the final character? (Hint: After writing your formula in column C, you can write a formula in cell C3 that uses the COUNTIFS function to count how many times the value in column C is 30.)

#### Answer located at: Data!C3

