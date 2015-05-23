
#Codebook for wearable computing dataset

#Variables

subject                    1..2
    Subject number
                           1..30 .Unique identifier assigned to each subject

label                      6..18
    Acitivity label
                           "WALKING"
                           "WALKING_UPSTAIRS"
                           "WALKING_DOWNSTAIRS"
                           "SITTING"
                           "STANDING"
                           "LAYING"

tbodyaccmeanx              12
    Described below

tbodyaccmeany              12
    Described below

tbodyaccmeanz              12
    Described below

tbodyaccstdx               12
    Described below

tbodyaccstdy               12
    Described below

tbodyaccstdz               12
    Described below

tgravityaccmeanx           12
    Described below

tgravityaccmeany           12
    Described below

tgravityaccmeanz           12
    Described below

tgravityaccstdx            12
    Described below

tgravityaccstdy            12
    Described below

tgravityaccstdz            12
    Described below

tbodyaccjerkmeanx          12
    Described below

tbodyaccjerkmeany          12
    Described below

tbodyaccjerkmeanz          12
    Described below

tbodyaccjerkstdx           12
    Described below

tbodyaccjerkstdy           12
    Described below

tbodyaccjerkstdz           12
    Described below

tbodygyromeanx             12
    Described below

tbodygyromeany             12
    Described below

tbodygyromeanz             12
    Described below

tbodygyrostdx              12
    Described below

tbodygyrostdy              12
    Described below

tbodygyrostdz              12
    Described below

tbodygyrojerkmeanx         12
    Described below

tbodygyrojerkmeany         12
    Described below

tbodygyrojerkmeanz         12
    Described below

tbodygyrojerkstdx          12
    Described below

tbodygyrojerkstdy          12
    Described below

tbodygyrojerkstdz          12
    Described below

tbodyaccmagmean            12
    Described below

tbodyaccmagstd             12
    Described below

tgravityaccmagmean         12
    Described below

tgravityaccmagstd          12
    Described below

tbodyaccjerkmagmean        12
    Described below

tbodyaccjerkmagstd         12
    Described below

tbodygyromagmean           12
    Described below

tbodygyromagstd            12
    Described below

tbodygyrojerkmagmean       12
    Described below

tbodygyrojerkmagstd        12
    Described below

fbodyaccmeanx              12
    Described below

fbodyaccmeany              12
    Described below

fbodyaccmeanz              12
    Described below

fbodyaccstdx               12
    Described below

fbodyaccstdy               12
    Described below

fbodyaccstdz               12
    Described below

fbodyaccjerkmeanx          12
    Described below

fbodyaccjerkmeany          12
    Described below

fbodyaccjerkmeanz          12
    Described below

fbodyaccjerkstdx           12
    Described below

fbodyaccjerkstdy           12
    Described below

fbodyaccjerkstdz           12
    Described below

fbodygyromeanx             12
    Described below

fbodygyromeany             12
    Described below

fbodygyromeanz             12
    Described below

fbodygyrostdx              12
    Described below

fbodygyrostdy              12
    Described below

fbodygyrostdz              12
    Described below

fbodyaccmagmean            12
    Described below

fbodyaccmagstd             12
    Described below

fbodybodyaccjerkmagmean    12
    Described below

fbodybodyaccjerkmagstd     12
    Described below

fbodybodygyromagmean       12
    Described below

fbodybodygyromagstd        12
    Described below

fbodybodygyrojerkmagmean   12
    Described below

fbodybodygyrojerkmagstd    12
    Described below

##Data

The dataset includes the following files:

'README.txt'

'features_info.txt': Shows information about the variables used on the feature vector.

'features.txt': List of all features.

'activity_labels.txt': Links the class labels with their activity name.

'train/X_train.txt': Training set.

'train/y_train.txt': Training labels.

'test/X_test.txt': Test set.

'test/y_test.txt': Test labels.

The following files are available for the train and test data. Their descriptions are equivalent.

'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.

'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis.

'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.

'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second
The set of variables that were estimated from these signals are:

mean: Mean value

std: Standard deviation

Transformation

##Transformation details

There are 5 parts:

Merges the training and the test sets to create one data set.  
Extracts only the measurements on the mean and standard deviation for each measurement.  
Uses descriptive activity names to name the activities in the data set.  
Appropriately labels the data set with descriptive activity names.   
Creates a second, independent tidy data set with the average of each variable for each activity and each subject.  