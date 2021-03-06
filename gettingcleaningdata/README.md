===========================================================================================================================
Getting and Cleaning Data Project John Hopkins Coursera
===========================================================================================================================

Additional information about the data base and files.

======================
 Database Information
======================

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. 
Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) 
wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, 
we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. 
The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly 
partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% 
the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled 
in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, 
which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body 
acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a 
filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating 
variables from the time and frequency domain. See 'features_info.txt' for more details. 

For each record it is provided:

- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.

=======
 Files
=======

The dataset includes the following files:

- 'run_analisys.R': Analysis R Script that generate the tidy data.
- 'README.md': Explains how all of the scripts work and how they are connected.
- 'CodeBook.md': Describes the variables, the data, and any transformations or work that you performed to clean up the data.
- 'tidyData.txt': Tidy data set generated by run_analisys.R
- 'tidyDataMean.txt': Tidy data set with the average of each variable for each activity and each subject.
- 'UCI HAR Dataset/features.txt': List of all features.
- 'UCI HAR Dataset/activity_labels.txt': Links the class labels with their activity name.
- 'UCI HAR Dataset/train/X_train.txt': Training set.
- 'UCI HAR Dataset/train/y_train.txt': Training labels.
- 'UCI HAR Dataset/train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample.
- 'UCI HAR Dataset/test/X_test.txt': Test set.
- 'UCI HAR Dataset/test/y_test.txt': Test labels.
- 'UCI HAR Dataset/test/subject_test.txt': Each row identifies the subject who performed the activity for each window sample.

=========
 License
=========

Anyone may contribute after this assignment is turned in and graded. 
