---
title: 'Echopath Software Engineering Intern Project'
date: 'January 3, 2025'
excerpt: 'This post will cover my work as a software engineering intern in the Fall 2024 semester'
cover_image: '/images/echopath/echopath.png'
---

# Echopath Software Engineering Intern

In Fall 2024, I was able to get a remote internship from Echopath LLC.  This remote internship allows me to work on my programming skills while getting advice and feedback from my mentor, both on career advice and the project itself.

## Echopath LLC

Echopath is an Indianapolis-based IT company that helps individuals and organizations manage their IT operations.  Founded in 2011, Echopath addresses several challenges and risks with critical aspects of IT such as security and backup.  They provide a comprehensive suite of IT services that can protect data and their systems.  To see more information, please visit their site <a href = "https://echopath.com/about-us/">here</a>.

## The Project

My project involved building a financial dashboard for the company leadership that takes in CSV files and appended them to an Excel file.  The CSV files had a specific structure that had to reformatted and added into an Excel file with several sheets.  The entire purpose of this project is important for every company: keep track of income and expense streams to ensure that the company systems are working as intended.

I will not show any code from this project due to the involvement of sensitive financial information.  However, what I can do is show what I have worked on in my internship so far.

![alt text](/images/echopath/menu.png)

As seen above in the image, once the program opens, there are five options: append historical data (data added to the first sheet called Historical Data), append projected data (data added to the second sheet called Financial Data), append actual data (data added to the second sheet called Financial Data), view sheets, and quit.  The way the program works is by selecting an option and then adding a specific file based on the type of data being added.

There are three types of CSV files being added: historical data, projected data, and actual data.  The historical data is a list of all of the data from previous years and acts as a record from previous years.  The projected data is data projecting the budget for an entire year while the actual data is meant to be used to compare how the budget is spent monthly.  For example, the actual data could show that the company saved some money in the first month, lost some money in the fifth month, and more.

There are also three sheets utilized in the Excel file: Historical Data, Financial Data, and Audit Log.  There is more information about these sheets down below.

## The First Sheet:  Historical Data

The historical data sheet has six categories:

- Account (un-trimmed): The income/expense type
- Timeframe: Month and year
- Amount: How much of the income/expense
- Account: The income-expense type but trimmed
- Datenumber: Year and month (in the format of YYYYMM)
- Date: Month and year

![alt text](/images/echopath/first-sheet.png)

As seen above in the image while also only focusing on the first six columns, the structure of this sheet was requested as a part of the first sheet.

## The Second Sheet: Financial Data

The financial data sheet has six categories:

- Account: The income/expense type for projected data
- Timeframe: Month and year for projected data
- Projected Amount: How much is projected to be for the income/expense
- Account: The income/expense type for actual data
- Timeframe: Month and year for actual data
- Actual Amount: How much was actually spent/made for the income/expense
- Difference: The difference between the projected and actual amounts

The first three columns were for the projected data while the next three columns were for the actual data.  Both of them were reformatted to match the three-column type.  The seventh column was requested to be added since it allows the leadership to see how much money they saved/lost based on their projected data and the actual amount for that specific income/expense type.  That way, it allowed them to make decisions based on this information.

## The Third Sheet: Audit Log

The audit log is meant to act as a record of what type of file has been added to the Excel file.  It has three columns:

- File Name: The name of the file being added
- Date & Time: The date and time at which the file was being added
- Data Type: The type of data being added (historical data, projected data, actual data)

## Technologies Utilized

This project involved utilizing Python and PyCharm to read CSV files.  The project works by clicking on a Windows Batch script, which will reveal a window with several options.

I utilized the pandas library to read a CSV file and append the data to the Excel file.  I also utilized the tkinter library to showcase a file selector to make it easier to select a file and the openpyxl library to read and write into the Excel file. 

## Other Features

Some safety measures have been added to the program to prevent it from crashing.  Some of the following safety measures include:

- Preventing the user from adding a duplicate file or file with the same data with hashcode
- Preventing the program from crashing if the Excel file is opened
- Preventing the user from adding actual data that does not have the corresponding projected data
- Preventing the program from crashing if a file has not been selected
- Made a basic confirm feature where it asks the user if the file they are adding is the file they want added or not

## Next Steps

The ultimate goal is to be able to build a dashboard in the Excel file with graphs and trends based on the data inserted in the Excel file.  The dashboard follows Pineapple Consulting's dashboard as seen below:

![alt text](/images/echopath/dashboard.png)

At the time of writing, this project is still ongoing and is subject to change.  If any other changes have occurred, I will write them down here.