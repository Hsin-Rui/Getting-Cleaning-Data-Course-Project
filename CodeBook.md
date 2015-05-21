# Course Project Introduction
The script `run_analysis.R` uses the `data.table` package for renaming column and reading in files. It performs 5 major steps including:


1. Merges the training and the test sets to create one data set. (In the following data means both train and test)
The `x_data.txt`, `y_data.txt`, `subject_data.txt` should be binded by row, and after that all three of them should binded by column.


2. Extracts only the measurements on the mean and standard deviation for each measurement. 
For the column of `x_data.txt`, extract only the ones that have mean() or std() in their names, compare it with `feature.txt`.


3. Uses descriptive activity names to name the activities in the data set
Match each number in the `y_data` column with `activity_labels.txt`


4. Appropriately labels the data set with descriptive variable names. 
Rename the column of `y_data` and `subject_data`, instead of using the default name given by R.


5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.   
Write out the tidt dataset to `averagedata.txt`.


# Data Introduction
- The data that will be used for this project are `x_train.txt`, `x_test.txt`, `y_train.txt`, `y_test.txt`, `subject_train.txt` and `subject_test.txt`, which can all be found inside the downloaded dataset **URI HAR Dataset**.
- `features.txt` contains the correct feature name, which corresponds to each column of `x_train.txt` and `x_test.txt`. Further explanation of the feature is in the `features_info.txt`. 
- `activity_labels.txt` contains the desciptive names for each activity label, which corresponds to each number in the `y_train.txt` and `y_test.txt`.
