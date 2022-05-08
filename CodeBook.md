# Getting and Cleaning Data Course Project

Here you'll find additional information about the variables, data, and transformations and work performed to clean up the data in the course project for the Johns Hopkins Getting and Cleaning Data course.

## Source

The Data Folder and the Data Set Description is available for download here:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## Data Set Information

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

## Attribute Information

For each record in the dataset it is provided:

- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope.
- A 561-feature vector with time and frequency domain variables.
- Its activity label.
- An identifier of the subject who carried out the experiment.

## Transformations

1) Read the files containing the labels for activities and features of the vector.

2) Read the test data.

    2.1) Read the data identifying subjects for test observations and rename columns.
    
    2.2) Read the data containing the feature list for test observations and add descriptions. 
    
    2.3) Read the data identifying type of activity for test observations and rename the  columns. 
    
    2.4) Column bind files under 2.1, 2.2 and 2.3 to get the complete table for the test observations.
    
    2.5) Keep only necessary columns, Subject.Id, Activity and columns containing mean in their description.
    
    2.6) Add the description for each activity type to produce the final test data for the observations.

3) Read the training data.

    3.1) Repeat steps 2.1 through 2.6 with the training data. 

4) Merge Training and Test Data to create one data set (training and test data have the same format, they will be bound vertically)

5) Reshape the merged data to produce the desired format for data aggregation.

    5.1) Use the melt function to prepare data for dcast aggregation.
    
    5.2) Aggregate data with dcast function to produce the final (tidy) data set

6) Finally write out to csv file the tidy data set in the Data folder.

