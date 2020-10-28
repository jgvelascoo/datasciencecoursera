#-----------------------------------------------------------------------
#-----------------------------------------------------------------------
#      Getting and Cleaning Data Project John Hopkins Coursera
#-----------------------------------------------------------------------
#-----------------------------------------------------------------------

#--------------
# Introduction
#--------------

Additional information about the variables, data and transformations used in the course project 
for the Johns Hopkins Getting and Cleaning Data course.

This code book is used for outlining the analyses to clean up the data and interpreting the variables 
in the tidyData.txt document

#---------------
# Source Data
#---------------

The data linked to from the course website represent data collected from the accelerometers from the 
Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

	http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Here are the data for the project:

	https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

#-------------------
# Analysis Pipeline
#-------------------

Part 1 - Merges the training and the test sets to create one data set

	# Read files in ./UCI HAR Dataset
	# Read files in ./UCI HAR Dataset/test
	# Read files in ./UCI HAR Dataset/train
	# Combine test data and set column names
	# Combine train data and set column names
	# Combine test and training data

Part 2 - Extracts only the measurements on the mean and standard deviation for each measurement.

	# Extracts features with mean and std [No include meanFreq()]

Part 3 - Uses descriptive activity names to name the activities in the data set

	# Change activity column by a factor of 6 levels, with the label the
	# same as the activity name

Part 4 - Appropriately labels the data set with descriptive variable names.

	# Remove the () for the mean and std in the measurements names
	# Create tidyData file

Part 5 - From the data set in step 4, creates a second, independent tidy data set with the average 
         of each variable for each activity and each subject.

	# Create tidyDataMean file

#-----------
# Variables
#-----------

Time signals and Frequency domain signals:

-   tBodyAcc-XYZ
-   tGravityAcc-XYZ
-   tBodyAccJerk-XYZ
-   tBodyGyro-XYZ
-   tBodyGyroJerk-XYZ
-   tBodyAccMag
-   tGravityAccMag
-   tBodyAccJerkMag
-   tBodyGyroMag
-   tBodyGyroJerkMag
-   fBodyAcc-XYZ
-   fBodyAccJerk-XYZ
-   fBodyGyro-XYZ
-   fBodyAccMag
-   fBodyAccJerkMag
-   fBodyGyroMag
-   fBodyGyroJerkMag

The set of variables that were estimated from these signals are as follows:

-   mean: Mean value
-   std: Standard deviation

Other variables:

-   subjectId: Identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.
-   activity: Six activities (WALKING, WALKING\_UPSTAIRS, WALKING\_DOWNSTAIRS, SITTING, STANDING, LAYING) 
              that the subjects performed wearing a smartphone (Samsung Galaxy S II) on the waist.

#------------------
# More Information
#------------------

Please see the README.md for more information