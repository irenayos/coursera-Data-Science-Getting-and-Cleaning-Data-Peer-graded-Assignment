# Getting and Cleaning Data - Peer-graded Assignment Project

Course project for Peer-graded Assignment. Getting and Cleaning Data Coursera course. 

R script run_analysis.R does the following:<br/>
* Download and unzip dataset https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
* Reads activity files
* Reads subject files
* Reads features files
* Combines data tables by rows
* Names the variables
* Merges the training and the test sets to create one dataset
* Extracts only the measurements on the mean and standard deviation for each measurement.
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names.
* From the dataset in step 4, creates a second, independent tidy dataset FinalData.txt, with the average of each variable for each activity and each subject.

Submission contains following files:
* CodeBook.md - describes original data source used in this assignment project
* TidyDataSet.txt - final output of run_analysis.R script execution
* Readme.md - short sumamrized description what I made to prepare TidyDataSet.txt file
* run_analysis.R - script I prepared to transform original dataset to TidyDataSet.txt data
