#Code Book

##The original data set information is splitted into several files they were produced by:
>=======================================
>Human Activity Recognition Using Smartphones Dataset
>
>Version 1.0
>
>======================================
>Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto.
>
>Smartlab - Non Linear Complex Systems Laboratory
>
>DITEN - Università degli Studi di Genova.
>
>Via Opera Pia 11A, I-16145, Genoa, Italy.
>
>activityrecognition@smartlab.ws
>
>www.smartlab.ws
>
>======================================

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. 

Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist.

The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The files used to generate the tidy data set result were:

* 'features.txt': List of all features.

* 'activity_labels.txt': Links the class labels with their activity name : WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING and LAYING

* 'train/X_train.txt' and 'test/X_test.txt': Training set and test set, features are normalized and bounded within [-1,1], 
   is a row on the set files is feature vector where the numeric values are separated by blanks

* 'train/y_train.txt' and 'test/y_test.txt': Test and Training labels, 

* 'train/subject_train.txt' and 'test/subject_test.txt': Each row identifies the subject who performed the activity for each window sample. activities range is from 1 to 30. 

The initial list of variables is (separated by ';' because some names contain ','):

    tBodyAcc-mean()-X; tBodyAcc-mean()-Y; tBodyAcc-mean()-Z; tBodyAcc-std()-X; tBodyAcc-std()-Y; tBodyAcc-std()-Z;
    tBodyAcc-mad()-X; tBodyAcc-mad()-Y; tBodyAcc-mad()-Z; tBodyAcc-max()-X; tBodyAcc-max()-Y; tBodyAcc-max()-Z;
    tBodyAcc-min()-X; tBodyAcc-min()-Y; tBodyAcc-min()-Z; tBodyAcc-sma(); tBodyAcc-energy()-X; tBodyAcc-energy()-Y;
    tBodyAcc-energy()-Z; tBodyAcc-iqr()-X; tBodyAcc-iqr()-Y; tBodyAcc-iqr()-Z; tBodyAcc-entropy()-X; tBodyAcc-entropy()-Y;
    tBodyAcc-entropy()-Z; tBodyAcc-arCoeff()-X,1; tBodyAcc-arCoeff()-X,2; tBodyAcc-arCoeff()-X,3; tBodyAcc-arCoeff()-X,4; tBodyAcc-arCoeff()-Y,1;
    tBodyAcc-arCoeff()-Y,2; tBodyAcc-arCoeff()-Y,3; tBodyAcc-arCoeff()-Y,4; tBodyAcc-arCoeff()-Z,1; tBodyAcc-arCoeff()-Z,2; tBodyAcc-arCoeff()-Z,3;
    tBodyAcc-arCoeff()-Z,4; tBodyAcc-correlation()-X,Y; tBodyAcc-correlation()-X,Z; tBodyAcc-correlation()-Y,Z; tGravityAcc-mean()-X; tGravityAcc-mean()-Y;
    tGravityAcc-mean()-Z; tGravityAcc-std()-X; tGravityAcc-std()-Y; tGravityAcc-std()-Z; tGravityAcc-mad()-X; tGravityAcc-mad()-Y;
    tGravityAcc-mad()-Z; tGravityAcc-max()-X; tGravityAcc-max()-Y; tGravityAcc-max()-Z; tGravityAcc-min()-X; tGravityAcc-min()-Y;
    tGravityAcc-min()-Z; tGravityAcc-sma(); tGravityAcc-energy()-X; tGravityAcc-energy()-Y; tGravityAcc-energy()-Z; tGravityAcc-iqr()-X;
    tGravityAcc-iqr()-Y; tGravityAcc-iqr()-Z; tGravityAcc-entropy()-X; tGravityAcc-entropy()-Y; tGravityAcc-entropy()-Z; tGravityAcc-arCoeff()-X,1;
    tGravityAcc-arCoeff()-X,2; tGravityAcc-arCoeff()-X,3; tGravityAcc-arCoeff()-X,4; tGravityAcc-arCoeff()-Y,1; tGravityAcc-arCoeff()-Y,2; tGravityAcc-arCoeff()-Y,3;
    tGravityAcc-arCoeff()-Y,4; tGravityAcc-arCoeff()-Z,1; tGravityAcc-arCoeff()-Z,2; tGravityAcc-arCoeff()-Z,3; tGravityAcc-arCoeff()-Z,4; tGravityAcc-correlation()-X,Y;
    tGravityAcc-correlation()-X,Z; tGravityAcc-correlation()-Y,Z; tBodyAccJerk-mean()-X; tBodyAccJerk-mean()-Y; tBodyAccJerk-mean()-Z; tBodyAccJerk-std()-X;
    tBodyAccJerk-std()-Y; tBodyAccJerk-std()-Z; tBodyAccJerk-mad()-X;tBodyAccJerk-mad()-Y; tBodyAccJerk-mad()-Z; tBodyAccJerk-max()-X;
    tBodyAccJerk-max()-Y; tBodyAccJerk-max()-Z; tBodyAccJerk-min()-X;tBodyAccJerk-min()-Y; tBodyAccJerk-min()-Z; tBodyAccJerk-sma();
    tBodyAccJerk-energy()-X; tBodyAccJerk-energy()-Y; tBodyAccJerk-energy()-Z; tBodyAccJerk-iqr()-X; tBodyAccJerk-iqr()-Y; tBodyAccJerk-iqr()-Z;
    tBodyAccJerk-entropy()-X; tBodyAccJerk-entropy()-Y; tBodyAccJerk-entropy()-Z; tBodyAccJerk-arCoeff()-X,1; tBodyAccJerk-arCoeff()-X,2; tBodyAccJerk-arCoeff()-X,3;
    tBodyAccJerk-arCoeff()-X,4; tBodyAccJerk-arCoeff()-Y,1; tBodyAccJerk-arCoeff()-Y,2; tBodyAccJerk-arCoeff()-Y,3; tBodyAccJerk-arCoeff()-Y,4; tBodyAccJerk-arCoeff()-Z,1;
    tBodyAccJerk-arCoeff()-Z,2; tBodyAccJerk-arCoeff()-Z,3; tBodyAccJerk-arCoeff()-Z,4; tBodyAccJerk-correlation()-X,Y; tBodyAccJerk-correlation()-X,Z; tBodyAccJerk-correlation()-Y,Z;
    tBodyGyro-mean()-X; tBodyGyro-mean()-Y; tBodyGyro-mean()-Z;tBodyGyro-std()-X; tBodyGyro-std()-Y; tBodyGyro-std()-Z;
    tBodyGyro-mad()-X; tBodyGyro-mad()-Y; tBodyGyro-mad()-Z;tBodyGyro-max()-X; tBodyGyro-max()-Y; tBodyGyro-max()-Z;
    tBodyGyro-min()-X; tBodyGyro-min()-Y; tBodyGyro-min()-Z;tBodyGyro-sma(); tBodyGyro-energy()-X; tBodyGyro-energy()-Y;
    tBodyGyro-energy()-Z; tBodyGyro-iqr()-X; tBodyGyro-iqr()-Y;tBodyGyro-iqr()-Z; tBodyGyro-entropy()-X; tBodyGyro-entropy()-Y;
    tBodyGyro-entropy()-Z; tBodyGyro-arCoeff()-X,1; tBodyGyro-arCoeff()-X,2;tBodyGyro-arCoeff()-X,3; tBodyGyro-arCoeff()-X,4; tBodyGyro-arCoeff()-Y,1;
    tBodyGyro-arCoeff()-Y,2; tBodyGyro-arCoeff()-Y,3; tBodyGyro-arCoeff()-Y,4;tBodyGyro-arCoeff()-Z,1; tBodyGyro-arCoeff()-Z,2; tBodyGyro-arCoeff()-Z,3;
    tBodyGyro-arCoeff()-Z,4; tBodyGyro-correlation()-X,Y; tBodyGyro-correlation()-X,Z;tBodyGyro-correlation()-Y,Z; tBodyGyroJerk-mean()-X; tBodyGyroJerk-mean()-Y;
    tBodyGyroJerk-mean()-Z; tBodyGyroJerk-std()-X; tBodyGyroJerk-std()-Y;tBodyGyroJerk-std()-Z; tBodyGyroJerk-mad()-X; tBodyGyroJerk-mad()-Y;
    tBodyGyroJerk-mad()-Z; tBodyGyroJerk-max()-X; tBodyGyroJerk-max()-Y;tBodyGyroJerk-max()-Z; tBodyGyroJerk-min()-X; tBodyGyroJerk-min()-Y;
    tBodyGyroJerk-min()-Z; tBodyGyroJerk-sma(); tBodyGyroJerk-energy()-X;tBodyGyroJerk-energy()-Y; tBodyGyroJerk-energy()-Z; tBodyGyroJerk-iqr()-X;
    tBodyGyroJerk-iqr()-Y; tBodyGyroJerk-iqr()-Z; tBodyGyroJerk-entropy()-X;tBodyGyroJerk-entropy()-Y; tBodyGyroJerk-entropy()-Z; tBodyGyroJerk-arCoeff()-X,1;
    tBodyGyroJerk-arCoeff()-X,2; tBodyGyroJerk-arCoeff()-X,3; tBodyGyroJerk-arCoeff()-X,4;tBodyGyroJerk-arCoeff()-Y,1; tBodyGyroJerk-arCoeff()-Y,2; tBodyGyroJerk-arCoeff()-Y,3;
    tBodyGyroJerk-arCoeff()-Y,4; tBodyGyroJerk-arCoeff()-Z,1; tBodyGyroJerk-arCoeff()-Z,2;tBodyGyroJerk-arCoeff()-Z,3; tBodyGyroJerk-arCoeff()-Z,4; tBodyGyroJerk-correlation()-X,Y;
    tBodyGyroJerk-correlation()-X,Z; tBodyGyroJerk-correlation()-Y,Z; tBodyAccMag-mean();tBodyAccMag-std(); tBodyAccMag-mad(); tBodyAccMag-max();
    tBodyAccMag-min(); tBodyAccMag-sma(); tBodyAccMag-energy();tBodyAccMag-iqr(); tBodyAccMag-entropy(); tBodyAccMag-arCoeff()1;
    tBodyAccMag-arCoeff()2; tBodyAccMag-arCoeff()3; tBodyAccMag-arCoeff()4;tGravityAccMag-mean(); tGravityAccMag-std(); tGravityAccMag-mad();
    tGravityAccMag-max(); tGravityAccMag-min(); tGravityAccMag-sma();tGravityAccMag-energy(); tGravityAccMag-iqr(); tGravityAccMag-entropy();
    tGravityAccMag-arCoeff()1; tGravityAccMag-arCoeff()2; tGravityAccMag-arCoeff()3;tGravityAccMag-arCoeff()4; tBodyAccJerkMag-mean(); tBodyAccJerkMag-std();
    tBodyAccJerkMag-mad(); tBodyAccJerkMag-max(); tBodyAccJerkMag-min();tBodyAccJerkMag-sma(); tBodyAccJerkMag-energy(); tBodyAccJerkMag-iqr();
    tBodyAccJerkMag-entropy(); tBodyAccJerkMag-arCoeff()1; tBodyAccJerkMag-arCoeff()2;tBodyAccJerkMag-arCoeff()3; tBodyAccJerkMag-arCoeff()4; tBodyGyroMag-mean();
    tBodyGyroMag-std(); tBodyGyroMag-mad(); tBodyGyroMag-max();tBodyGyroMag-min(); tBodyGyroMag-sma(); tBodyGyroMag-energy();
    tBodyGyroMag-iqr(); tBodyGyroMag-entropy(); tBodyGyroMag-arCoeff()1;tBodyGyroMag-arCoeff()2; tBodyGyroMag-arCoeff()3; tBodyGyroMag-arCoeff()4;
    tBodyGyroJerkMag-mean(); tBodyGyroJerkMag-std(); tBodyGyroJerkMag-mad();tBodyGyroJerkMag-max(); tBodyGyroJerkMag-min(); tBodyGyroJerkMag-sma();
    tBodyGyroJerkMag-energy(); tBodyGyroJerkMag-iqr(); tBodyGyroJerkMag-entropy();tBodyGyroJerkMag-arCoeff()1; tBodyGyroJerkMag-arCoeff()2; tBodyGyroJerkMag-arCoeff()3;
    tBodyGyroJerkMag-arCoeff()4; fBodyAcc-mean()-X; fBodyAcc-mean()-Y;fBodyAcc-mean()-Z; fBodyAcc-std()-X; fBodyAcc-std()-Y;
    fBodyAcc-std()-Z; fBodyAcc-mad()-X; fBodyAcc-mad()-Y;fBodyAcc-mad()-Z; fBodyAcc-max()-X; fBodyAcc-max()-Y;
    fBodyAcc-max()-Z; fBodyAcc-min()-X; fBodyAcc-min()-Y;fBodyAcc-min()-Z; fBodyAcc-sma(); fBodyAcc-energy()-X;
    fBodyAcc-energy()-Y; fBodyAcc-energy()-Z; fBodyAcc-iqr()-X;fBodyAcc-iqr()-Y; fBodyAcc-iqr()-Z; fBodyAcc-entropy()-X;
    fBodyAcc-entropy()-Y; fBodyAcc-entropy()-Z; fBodyAcc-maxInds-X;fBodyAcc-maxInds-Y; fBodyAcc-maxInds-Z; fBodyAcc-meanFreq()-X;
    fBodyAcc-meanFreq()-Y; fBodyAcc-meanFreq()-Z; fBodyAcc-skewness()-X;fBodyAcc-kurtosis()-X; fBodyAcc-skewness()-Y; fBodyAcc-kurtosis()-Y;
    fBodyAcc-skewness()-Z; fBodyAcc-kurtosis()-Z; fBodyAcc-bandsEnergy()-1,8;fBodyAcc-bandsEnergy()-9,16; fBodyAcc-bandsEnergy()-17,24; fBodyAcc-bandsEnergy()-25,32;
    fBodyAcc-bandsEnergy()-33,40; fBodyAcc-bandsEnergy()-41,48; fBodyAcc-bandsEnergy()-49,56;fBodyAcc-bandsEnergy()-57,64; fBodyAcc-bandsEnergy()-1,16; fBodyAcc-bandsEnergy()-17,32;
    fBodyAcc-bandsEnergy()-33,48; fBodyAcc-bandsEnergy()-49,64; fBodyAcc-bandsEnergy()-1,24;fBodyAcc-bandsEnergy()-25,48; fBodyAcc-bandsEnergy()-1,8; fBodyAcc-bandsEnergy()-9,16;
    fBodyAcc-bandsEnergy()-17,24; fBodyAcc-bandsEnergy()-25,32; fBodyAcc-bandsEnergy()-33,40;fBodyAcc-bandsEnergy()-41,48; fBodyAcc-bandsEnergy()-49,56; fBodyAcc-bandsEnergy()-57,64;
    fBodyAcc-bandsEnergy()-1,16; fBodyAcc-bandsEnergy()-17,32; fBodyAcc-bandsEnergy()-33,48;fBodyAcc-bandsEnergy()-49,64; fBodyAcc-bandsEnergy()-1,24; fBodyAcc-bandsEnergy()-25,48;
    fBodyAcc-bandsEnergy()-1,8; fBodyAcc-bandsEnergy()-9,16; fBodyAcc-bandsEnergy()-17,24;fBodyAcc-bandsEnergy()-25,32; fBodyAcc-bandsEnergy()-33,40; fBodyAcc-bandsEnergy()-41,48;
    fBodyAcc-bandsEnergy()-49,56; fBodyAcc-bandsEnergy()-57,64; fBodyAcc-bandsEnergy()-1,16;fBodyAcc-bandsEnergy()-17,32; fBodyAcc-bandsEnergy()-33,48; fBodyAcc-bandsEnergy()-49,64;
    fBodyAcc-bandsEnergy()-1,24; fBodyAcc-bandsEnergy()-25,48; fBodyAccJerk-mean()-X;fBodyAccJerk-mean()-Y; fBodyAccJerk-mean()-Z; fBodyAccJerk-std()-X;
    fBodyAccJerk-std()-Y; fBodyAccJerk-std()-Z; fBodyAccJerk-mad()-X;fBodyAccJerk-mad()-Y; fBodyAccJerk-mad()-Z; fBodyAccJerk-max()-X;
    fBodyAccJerk-max()-Y; fBodyAccJerk-max()-Z; fBodyAccJerk-min()-X;fBodyAccJerk-min()-Y; fBodyAccJerk-min()-Z; fBodyAccJerk-sma();
    fBodyAccJerk-energy()-X; fBodyAccJerk-energy()-Y; fBodyAccJerk-energy()-Z;fBodyAccJerk-iqr()-X; fBodyAccJerk-iqr()-Y; fBodyAccJerk-iqr()-Z;
    fBodyAccJerk-entropy()-X; fBodyAccJerk-entropy()-Y; fBodyAccJerk-entropy()-Z;fBodyAccJerk-maxInds-X; fBodyAccJerk-maxInds-Y; fBodyAccJerk-maxInds-Z;
    fBodyAccJerk-meanFreq()-X; fBodyAccJerk-meanFreq()-Y; fBodyAccJerk-meanFreq()-Z;fBodyAccJerk-skewness()-X; fBodyAccJerk-kurtosis()-X; fBodyAccJerk-skewness()-Y;
    fBodyAccJerk-kurtosis()-Y; fBodyAccJerk-skewness()-Z; fBodyAccJerk-kurtosis()-Z;fBodyAccJerk-bandsEnergy()-1,8; fBodyAccJerk-bandsEnergy()-9,16; fBodyAccJerk-bandsEnergy()-17,24;
    fBodyAccJerk-bandsEnergy()-25,32; fBodyAccJerk-bandsEnergy()-33,40; fBodyAccJerk-bandsEnergy()-41,48;fBodyAccJerk-bandsEnergy()-49,56; fBodyAccJerk-bandsEnergy()-57,64; fBodyAccJerk-bandsEnergy()-1,16;
    fBodyAccJerk-bandsEnergy()-17,32; fBodyAccJerk-bandsEnergy()-33,48; fBodyAccJerk-bandsEnergy()-49,64;fBodyAccJerk-bandsEnergy()-1,24; fBodyAccJerk-bandsEnergy()-25,48; fBodyAccJerk-bandsEnergy()-1,8;
    fBodyAccJerk-bandsEnergy()-9,16; fBodyAccJerk-bandsEnergy()-17,24; fBodyAccJerk-bandsEnergy()-25,32;fBodyAccJerk-bandsEnergy()-33,40; fBodyAccJerk-bandsEnergy()-41,48; fBodyAccJerk-bandsEnergy()-49,56;
    fBodyAccJerk-bandsEnergy()-57,64; fBodyAccJerk-bandsEnergy()-1,16; fBodyAccJerk-bandsEnergy()-17,32;fBodyAccJerk-bandsEnergy()-33,48; fBodyAccJerk-bandsEnergy()-49,64; fBodyAccJerk-bandsEnergy()-1,24;
    fBodyAccJerk-bandsEnergy()-25,48; fBodyAccJerk-bandsEnergy()-1,8; fBodyAccJerk-bandsEnergy()-9,16;fBodyAccJerk-bandsEnergy()-17,24; fBodyAccJerk-bandsEnergy()-25,32; fBodyAccJerk-bandsEnergy()-33,40;
    fBodyAccJerk-bandsEnergy()-41,48; fBodyAccJerk-bandsEnergy()-49,56; fBodyAccJerk-bandsEnergy()-57,64;fBodyAccJerk-bandsEnergy()-1,16; fBodyAccJerk-bandsEnergy()-17,32; fBodyAccJerk-bandsEnergy()-33,48;
    fBodyAccJerk-bandsEnergy()-49,64; fBodyAccJerk-bandsEnergy()-1,24; fBodyAccJerk-bandsEnergy()-25,48;fBodyGyro-mean()-X; fBodyGyro-mean()-Y; fBodyGyro-mean()-Z;
    fBodyGyro-std()-X; fBodyGyro-std()-Y; fBodyGyro-std()-Z;fBodyGyro-mad()-X; fBodyGyro-mad()-Y; fBodyGyro-mad()-Z;
    fBodyGyro-max()-X; fBodyGyro-max()-Y; fBodyGyro-max()-Z;fBodyGyro-min()-X; fBodyGyro-min()-Y; fBodyGyro-min()-Z;
    fBodyGyro-sma(); fBodyGyro-energy()-X; fBodyGyro-energy()-Y;fBodyGyro-energy()-Z; fBodyGyro-iqr()-X; fBodyGyro-iqr()-Y;
    fBodyGyro-iqr()-Z; fBodyGyro-entropy()-X; fBodyGyro-entropy()-Y;fBodyGyro-entropy()-Z; fBodyGyro-maxInds-X; fBodyGyro-maxInds-Y;
    fBodyGyro-maxInds-Z; fBodyGyro-meanFreq()-X; fBodyGyro-meanFreq()-Y;fBodyGyro-meanFreq()-Z; fBodyGyro-skewness()-X; fBodyGyro-kurtosis()-X;
    fBodyGyro-skewness()-Y; fBodyGyro-kurtosis()-Y; fBodyGyro-skewness()-Z;fBodyGyro-kurtosis()-Z; fBodyGyro-bandsEnergy()-1,8; fBodyGyro-bandsEnergy()-9,16;
    fBodyGyro-bandsEnergy()-17,24; fBodyGyro-bandsEnergy()-25,32; fBodyGyro-bandsEnergy()-33,40;fBodyGyro-bandsEnergy()-41,48; fBodyGyro-bandsEnergy()-49,56; fBodyGyro-bandsEnergy()-57,64;
    fBodyGyro-bandsEnergy()-1,16; fBodyGyro-bandsEnergy()-17,32; fBodyGyro-bandsEnergy()-33,48;fBodyGyro-bandsEnergy()-49,64; fBodyGyro-bandsEnergy()-1,24; fBodyGyro-bandsEnergy()-25,48;
    fBodyGyro-bandsEnergy()-1,8; fBodyGyro-bandsEnergy()-9,16; fBodyGyro-bandsEnergy()-17,24;fBodyGyro-bandsEnergy()-25,32; fBodyGyro-bandsEnergy()-33,40; fBodyGyro-bandsEnergy()-41,48;
    fBodyGyro-bandsEnergy()-49,56; fBodyGyro-bandsEnergy()-57,64; fBodyGyro-bandsEnergy()-1,16;fBodyGyro-bandsEnergy()-17,32; fBodyGyro-bandsEnergy()-33,48; fBodyGyro-bandsEnergy()-49,64;
    fBodyGyro-bandsEnergy()-1,24; fBodyGyro-bandsEnergy()-25,48; fBodyGyro-bandsEnergy()-1,8;fBodyGyro-bandsEnergy()-9,16; fBodyGyro-bandsEnergy()-17,24; fBodyGyro-bandsEnergy()-25,32;
    fBodyGyro-bandsEnergy()-33,40; fBodyGyro-bandsEnergy()-41,48; fBodyGyro-bandsEnergy()-49,56;fBodyGyro-bandsEnergy()-57,64; fBodyGyro-bandsEnergy()-1,16; fBodyGyro-bandsEnergy()-17,32;
    fBodyGyro-bandsEnergy()-33,48; fBodyGyro-bandsEnergy()-49,64; fBodyGyro-bandsEnergy()-1,24;fBodyGyro-bandsEnergy()-25,48; fBodyAccMag-mean(); fBodyAccMag-std();
    fBodyAccMag-mad(); fBodyAccMag-max(); fBodyAccMag-min();fBodyAccMag-sma(); fBodyAccMag-energy(); fBodyAccMag-iqr();
    fBodyAccMag-entropy(); fBodyAccMag-maxInds; fBodyAccMag-meanFreq();fBodyAccMag-skewness(); fBodyAccMag-kurtosis(); fBodyBodyAccJerkMag-mean();
    fBodyBodyAccJerkMag-std(); fBodyBodyAccJerkMag-mad(); fBodyBodyAccJerkMag-max();fBodyBodyAccJerkMag-min(); fBodyBodyAccJerkMag-sma(); fBodyBodyAccJerkMag-energy();
    fBodyBodyAccJerkMag-iqr(); fBodyBodyAccJerkMag-entropy(); fBodyBodyAccJerkMag-maxInds;fBodyBodyAccJerkMag-meanFreq(); fBodyBodyAccJerkMag-skewness(); fBodyBodyAccJerkMag-kurtosis();
    fBodyBodyGyroMag-mean(); fBodyBodyGyroMag-std(); fBodyBodyGyroMag-mad();fBodyBodyGyroMag-max(); fBodyBodyGyroMag-min(); fBodyBodyGyroMag-sma();
    fBodyBodyGyroMag-energy(); fBodyBodyGyroMag-iqr(); fBodyBodyGyroMag-entropy();fBodyBodyGyroMag-maxInds; fBodyBodyGyroMag-meanFreq(); fBodyBodyGyroMag-skewness();
    fBodyBodyGyroMag-kurtosis(); fBodyBodyGyroJerkMag-mean(); fBodyBodyGyroJerkMag-std();fBodyBodyGyroJerkMag-mad(); fBodyBodyGyroJerkMag-max(); fBodyBodyGyroJerkMag-min();
    fBodyBodyGyroJerkMag-sma(); fBodyBodyGyroJerkMag-energy(); fBodyBodyGyroJerkMag-iqr();fBodyBodyGyroJerkMag-entropy(); fBodyBodyGyroJerkMag-maxInds; fBodyBodyGyroJerkMag-meanFreq();
    fBodyBodyGyroJerkMag-skewness(); fBodyBodyGyroJerkMag-kurtosis(); angle(tBodyAccMean,gravity);angle(tBodyAccJerkMean),gravityMean); angle(tBodyGyroMean,gravityMean); angle(tBodyGyroJerkMean,gravityMean);
    angle(X,gravityMean); angle(Y,gravityMean); angle(Z,gravityMean)

###Transformations on the firsts data sets
The data set rows are appended x_train with x_test, subject_train with  subject_test and y_train with y_test.

Only the features containing mean and standard deviation computations are retained, this 66 features instead of 561.

The resulting extracted features are:

    tBodyAcc-mean()-X;          tBodyAcc-mean()-Y;          tBodyAcc-mean()-Z;         
    tBodyAcc-std()-X;           tBodyAcc-std()-Y;           tBodyAcc-std()-Z;          
    tGravityAcc-mean()-X;       tGravityAcc-mean()-Y;       tGravityAcc-mean()-Z;      
    tGravityAcc-std()-X;        tGravityAcc-std()-Y;        tGravityAcc-std()-Z;       
    tBodyAccJerk-mean()-X;      tBodyAccJerk-mean()-Y;      tBodyAccJerk-mean()-Z;     
    tBodyAccJerk-std()-X;       tBodyAccJerk-std()-Y;       tBodyAccJerk-std()-Z;      
    tBodyGyro-mean()-X;         tBodyGyro-mean()-Y;         tBodyGyro-mean()-Z;        
    tBodyGyro-std()-X;          tBodyGyro-std()-Y;          tBodyGyro-std()-Z;         
    tBodyGyroJerk-mean()-X;     tBodyGyroJerk-mean()-Y;     tBodyGyroJerk-mean()-Z;    
    tBodyGyroJerk-std()-X;      tBodyGyroJerk-std()-Y;      tBodyGyroJerk-std()-Z;     
    tBodyAccMag-mean();         tBodyAccMag-std();          tGravityAccMag-mean();     
    tGravityAccMag-std();       tBodyAccJerkMag-mean();     tBodyAccJerkMag-std();     
    tBodyGyroMag-mean();        tBodyGyroMag-std();         tBodyGyroJerkMag-mean();   
    tBodyGyroJerkMag-std();     fBodyAcc-mean()-X;          fBodyAcc-mean()-Y;         
    fBodyAcc-mean()-Z;          fBodyAcc-std()-X;           fBodyAcc-std()-Y;          
    fBodyAcc-std()-Z;           fBodyAccJerk-mean()-X;      fBodyAccJerk-mean()-Y;     
    fBodyAccJerk-mean()-Z;      fBodyAccJerk-std()-X;       fBodyAccJerk-std()-Y;      
    fBodyAccJerk-std()-Z;       fBodyGyro-mean()-X;         fBodyGyro-mean()-Y;        
    fBodyGyro-mean()-Z;         fBodyGyro-std()-X;          fBodyGyro-std()-Y;         
    fBodyGyro-std()-Z;          fBodyAccMag-mean();         fBodyAccMag-std();         
    fBodyBodyAccJerkMag-mean(); fBodyBodyAccJerkMag-std();  fBodyBodyGyroMag-mean();   
    fBodyBodyGyroMag-std();     fBodyBodyGyroJerkMag-mean();fBodyBodyGyroJerkMag-std()

The subject data set is added as the feature "subject" to the data set extraction.

The activity values (range 1:6) on the y data set are replaced by their corresponding labels and added as the activity feature to the extracted data set.

To have names with only alphanumeric characters, symbols '-','(',and ')' are deleted.

The data set resulting names for the 68 features are:

    tBodyAccmeanX,           tBodyAccmeanY,           tBodyAccmeanZ,          
    tBodyAccstdX,            tBodyAccstdY,            tBodyAccstdZ,           
    tGravityAccmeanX,        tGravityAccmeanY,        tGravityAccmeanZ,       
    tGravityAccstdX,         tGravityAccstdY,         tGravityAccstdZ,        
    tBodyAccJerkmeanX,       tBodyAccJerkmeanY,       tBodyAccJerkmeanZ,      
    tBodyAccJerkstdX,        tBodyAccJerkstdY,        tBodyAccJerkstdZ,       
    tBodyGyromeanX,          tBodyGyromeanY,          tBodyGyromeanZ,         
    tBodyGyrostdX,           tBodyGyrostdY,           tBodyGyrostdZ,          
    tBodyGyroJerkmeanX,      tBodyGyroJerkmeanY,      tBodyGyroJerkmeanZ,     
    tBodyGyroJerkstdX,       tBodyGyroJerkstdY,       tBodyGyroJerkstdZ,      
    tBodyAccMagmean,         tBodyAccMagstd,          tGravityAccMagmean,     
    tGravityAccMagstd,       tBodyAccJerkMagmean,     tBodyAccJerkMagstd,     
    tBodyGyroMagmean,        tBodyGyroMagstd,         tBodyGyroJerkMagmean,   
    tBodyGyroJerkMagstd,     fBodyAccmeanX,           fBodyAccmeanY,          
    fBodyAccmeanZ,           fBodyAccstdX,            fBodyAccstdY,           
    fBodyAccstdZ,            fBodyAccJerkmeanX,       fBodyAccJerkmeanY,      
    fBodyAccJerkmeanZ,       fBodyAccJerkstdX,        fBodyAccJerkstdY,       
    fBodyAccJerkstdZ,        fBodyGyromeanX,          fBodyGyromeanY,         
    fBodyGyromeanZ,          fBodyGyrostdX,           fBodyGyrostdY,          
    fBodyGyrostdZ,           fBodyAccMagmean,         fBodyAccMagstd,         
    fBodyBodyAccJerkMagmean, fBodyBodyAccJerkMagstd,  fBodyBodyGyroMagmean,   
    fBodyBodyGyroMagstd,     fBodyBodyGyroJerkMagmean,fBodyBodyGyroJerkMagstd,
    activity,                subject

##Operations to create the tidy data set
###A tidy data set is made of a group by on activity and subject features and for this grouping the average of all other variables is computed.

The names of the tidy set features are changed to reflect the average computation. The data set names are:

    activity,                subject,
    tBodyAccmeanX.mean,           tBodyAccmeanY.mean,           tBodyAccmeanZ.mean,          
    tBodyAccstdX.mean,            tBodyAccstdY.mean,            tBodyAccstdZ.mean,           
    tGravityAccmeanX.mean,        tGravityAccmeanY.mean,        tGravityAccmeanZ.mean,       
    tGravityAccstdX.mean,         tGravityAccstdY.mean,         tGravityAccstdZ.mean,        
    tBodyAccJerkmeanX.mean,       tBodyAccJerkmeanY.mean,       tBodyAccJerkmeanZ.mean,      
    tBodyAccJerkstdX.mean,        tBodyAccJerkstdY.mean,        tBodyAccJerkstdZ.mean,       
    tBodyGyromeanX.mean,          tBodyGyromeanY.mean,          tBodyGyromeanZ.mean,         
    tBodyGyrostdX.mean,           tBodyGyrostdY.mean,           tBodyGyrostdZ.mean,          
    tBodyGyroJerkmeanX.mean,      tBodyGyroJerkmeanY.mean,      tBodyGyroJerkmeanZ.mean,     
    tBodyGyroJerkstdX.mean,       tBodyGyroJerkstdY.mean,       tBodyGyroJerkstdZ.mean,      
    tBodyAccMagmean.mean,         tBodyAccMagstd.mean,          tGravityAccMagmean.mean,     
    tGravityAccMagstd.mean,       tBodyAccJerkMagmean.mean,     tBodyAccJerkMagstd.mean,     
    tBodyGyroMagmean.mean,        tBodyGyroMagstd.mean,         tBodyGyroJerkMagmean.mean,   
    tBodyGyroJerkMagstd.mean,     fBodyAccmeanX.mean,           fBodyAccmeanY.mean,          
    fBodyAccmeanZ.mean,           fBodyAccstdX.mean,            fBodyAccstdY.mean,           
    fBodyAccstdZ.mean,            fBodyAccJerkmeanX.mean,       fBodyAccJerkmeanY.mean,      
    fBodyAccJerkmeanZ.mean,       fBodyAccJerkstdX.mean,        fBodyAccJerkstdY.mean,       
    fBodyAccJerkstdZ.mean,        fBodyGyromeanX.mean,          fBodyGyromeanY.mean,         
    fBodyGyromeanZ.mean,          fBodyGyrostdX.mean,           fBodyGyrostdY.mean,              
    fBodyGyrostdZ.mean,           fBodyAccMagmean.mean,         fBodyAccMagstd.mean,         
    fBodyBodyAccJerkMagmean.mean, fBodyBodyAccJerkMagstd.mean,  fBodyBodyGyroMagmean.mean,   
    fBodyBodyGyroMagstd.mean,     fBodyBodyGyroJerkMagmean.mean,fBodyBodyGyroJerkMagstd.mean



