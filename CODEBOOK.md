Getting-and-Cleaning-Data-Project
=================================

## Steps followed in cleaning the data

### Dataset used : [Click Here to download](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)
### Dataset reference : [Click Here to visit](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

- Firstly we create a merged data set by reading training and test data files from train and test folder. Here we merge measurement data, subject information and activity related data.
- Then to extract only the measurements on the mean and standard deviation for each measurement we read `features.txt`and assign these names to the measurement data set.
- Then by a similar process we add activity labels which are in lower case and free of underscores and parenthesis and subject IDs.
- Finally, the script creates a 2nd, independent tidy data set with the average of each measurement for each activity and each subject. The resultant data set is saved in the working directory with the file name `tidydataset.txt`, the first column has subject IDs, the second column has activity names (walking, walkingupstairs, walkingdownstairs, sitting, standing, laying) and then the averages for each of the 66 attributes are in remaining columns. There are 30 subjects and 6 activities, thus 180 rows in the final tidy dataset.

 
