Tidy DataSet CodeBook
=====================

run_analysis.R script downloads data from predefined url, prepares data and performs 5 steps required by the assignment:
* Merges the training and the test sets to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement.
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names.
* From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

Data source
-----------
Tidy DataSet is derived from the "Human Activity Recognition Using Smartphones Data Set", which is avaiable here: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Feature Selection 
-----------------
README and features.txt files of original zip file describe original dataset:

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ<br/>
tGravityAcc-XYZ<br/>
tBodyAccJerk-XYZ<br/>
tBodyGyro-XYZ<br/>
tBodyGyroJerk-XYZ<br/>
tBodyAccMag<br/>
tGravityAccMag<br/>
tBodyAccJerkMag<br/>
tBodyGyroMag<br/>
tBodyGyroJerkMag<br/>
fBodyAcc-XYZ<br/>
fBodyAccJerk-XYZ<br/>
fBodyGyro-XYZ<br/>
fBodyAccMag<br/>
fBodyAccJerkMag<br/>
fBodyGyroMag<br/>
fBodyGyroJerkMag<br/>

The set of variables that were estimated from these signals are: 

mean(): Mean value<br/>
std(): Standard deviation<br/>
mad(): Median absolute deviation<br/> 
max(): Largest value in array<br/>
min(): Smallest value in array<br/>
sma(): Signal magnitude area<br/>
energy(): Energy measure. Sum of the squares divided by the number of values. <br/>
iqr(): Interquartile range <br/>
entropy(): Signal entropy<br/>
arCoeff(): Autorregresion coefficients with Burg order equal to 4<br/>
correlation(): correlation coefficient between two signals<br/>
maxInds(): index of the frequency component with largest magnitude<br/>
meanFreq(): Weighted average of the frequency components to obtain a mean frequency<br/>
skewness(): skewness of the frequency domain signal <br/>
kurtosis(): kurtosis of the frequency domain signal <br/>
bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.<br/>
angle(): Angle between to vectors.<br/>

Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable:

gravityMean<br/>
tBodyAccMean<br/>
tBodyAccJerkMean<br/>
tBodyGyroMean<br/>
tBodyGyroJerkMean<br/>

Final Tidy DataSet contains 180 rows, 30 subjects per 6 activities.
