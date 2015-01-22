# Getting-and-Cleaning-Data---Course-Project

The goal if this project is to prepare tidy data set. 

This is the data analyzed in this project:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

For this project I:
- Merged the training and the test sets to create one data set.
- Extracted the measurements on the mean and standard deviation for each measurement. 
- Used descriptive activity names to name the activities in the data set
- Appropriately labeled the data set with descriptive variable names. 

I then created a second, independent tidy data set with the average of each variable for each activity and each subject.

The features are unlabeled and can be found in the x_test.txt. The activity labels are in the 

y_test.txt file. The test subjects are in the subject_test.txt file.

I created a script called run_analysis.R which will merge the test and training sets together. Prerequisites for 
this script:

    the UCI HAR Dataset must be extracted and..
    the UCI HAR Dataset must be availble in a directory called "UCI HAR Dataset"

After merging testing and training, labels are added and only columns that have to do with mean and standarddeviation are kept. Lastly, the script will create a tidy data set containing the means of all the columns per test subject and per activity. This tidy dataset will be written to a tab-delimited file called tidy.txt, which can also be found in this repository.

About the Code Book

The CodeBook.md file explains the transformations performed and the resulting data and variables.
