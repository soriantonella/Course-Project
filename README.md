# Getting and Cleaning Data Project

The purpose of this project is to demonstrate my ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. 
The data used in this project represents data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

The data used in this project is available for download here: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip  

## Components 

Script | Item | Link to Item
--- | --- | ---
GitHub Repo | Repo |  [Repo Link](https://github.com/soriantonella/Course_Project "Click to go to Repo")
README | Current File |  [README Link](https://github.com/soriantonella/Course_Project/blob/main/README.md "README.md")
CodeBook | CodeBook.md |  [CodeBook link](https://github.com/mGalarnyk/datasciencecoursera/blob/master/3_Getting_and_Cleaning_Data/projects/CodeBook.md "CodeBook.md")
Analysis R Script |  run_analysis.R |  [R Script Link](https://github.com/mGalarnyk/datasciencecoursera/blob/master/3_Getting_and_Cleaning_Data/projects/run_analysis.R "run_analysis.R")
Tidy Data Set |  Clean Data Set |  [Data Set Link](https://github.com/mGalarnyk/datasciencecoursera/blob/master/3_Getting_and_Cleaning_Data/data/tidyData.txt "tidyData.txt")

- CodeBook.md -> Markdown file that describes the variables, the data, and any transformations or work performed to clean up the data.
- run_analysis.R ->	Script that contains all the actions taken to process the data. The script does the following
    - Merges the training and the test sets to create one data set.
    - Extracts only the measurements on the mean and standard deviation for each measurement. 
    - Uses descriptive activity names to name the activities in the data set.
    - Appropriately labels the data set with descriptive variable names. 
    - From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
- tidydataset.txt -> Text file that contains the tidy data set. 
