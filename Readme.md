## Getting and cleaning data project

### run_analysis.R script

`run_analysis.R` script uses "Human Activity Recognition Using Smartphones Data Set" 
information to create a new tidy date set according to Coursera - Getting and 
Cleaning Data course project.

`run_analysis.R` identifies subject and activity in train and test observations, 
then puts train and test data together. This script insolates mean an standard 
deviation measurements and assigns descriptive names to variables. It calculates 
the average of each measurement aggregating it by activity for every subject. Finally, 
it saves the resulting tidy data set on a file.

This script must be placed in the same path as `./data` directory.

Input files:

from `./data/` directory: 
  * features.txt
  * activity_labels.txt
  
from `./data/train/` directory:  
  * X_train.txt
  * y_train.txt
  * subject_train.txt
  
from `./data/test/` directory:
  * X_test.txt
  * y_test.txt
  * subject_test.txt

Output file:

  * tidy_DT.txt


### CodeBook.md

This document describes the transformations `run_analysis.R` performs over the 
train and test data sets in order to get a processed tidy data set.
The variables and observations from the resulting tidy data set are also described.