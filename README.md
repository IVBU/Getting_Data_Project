# Getting_Data_Project

Explanations for Getting Data Project R script:

The R script (run_analysis.R) that you can find in this repository produces tidy datasets as follows:
1.	Merges the training and test datasets to create one data set. The training datasets can be found in: train directory (X_train.txt , subject_train.txt , and y_train.txt ) and the test datasets can be found in test directory (X_test.txt, subject_test.txt, and y_test.txt) for
a.	Number of instances = 10,299 (x)
b.	Number of Attributes = 561 (x)
c.	Number of subject IDs = 10,299 (Sub)
d.	Number of activities = 10,299 (y)
2.	The script reads the features.txt and extracts the mean and the standard deviation for each measurement. 
3.	Then it reads the activity_labels and gives activity names like (walking, walkingupstairs, walkingupstairs, sitting, standing, laying)
4.	The script then labels the dataset with descriptive names, the attributes (feature names) and activity names are written in lowercase and underscores and () are removed. Then it merges the 10299x66 data frame of features with 10299x1 data frame(s) of activity labels and subject IDs. The result is saved as first_merged_tidy_dataset.txt, a 10299x68 data frame such that the first column contains subject IDs, the second column activity names, and the last 66 columns are measurements. Subject IDs are integers between 1 and 30 inclusive. The names of the attributes are (tbodyacc-mean-x , tbodyacc-mean-y, tbodyacc-mean-z, tbodyacc-std-x, tbodyacc-std-y, tbodyacc-std-z, 	tgravityacc-mean-x, tgravityacc-mean-y, etc.)
5.	The script then creates a second, independent tidy data set, with the average of each measurement for each activity and each subject. The result is saved as second_tidy_dataset_with_averages.txt, a 180x68 data frame, where the first column contains subject IDs, the second column contains activity names, and the averages for each of the 66 attributes are in columns 3 to 68. There are 30 subjects and 6 activities, thus 180 rows in this data set with averages.

