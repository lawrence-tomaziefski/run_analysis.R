# Getting and Cleaning Data
Use the provided run_analysis.R file and the corresponding code book to build a tidy data set.  
#####Project Requirement
Create one R script called run_analysis.R that does the following:





        1. Merges the training and the test sets to create one data set.
        2. Extracts only the measurements on the mean and standard deviation
        for each measurement.
        3. Uses descriptive activity names to name the activities in the data 
        set.
        4. Appropriately labels the data set with descriptive variable names.
        5. From the data set in step 4 creates a second, independent tidy data 
        set with the average of each variable for each activity and each subject.
#####General Approach
Keeping the fundamental goal of making tidy data in mind, my approach was to ensure 
that:



        1. Each variable forms a column and each observation forms a row.
        2. Variable names are: 
        i)  Lower case. 
        ii) Descriptive.
        iii) Do not contain any special characters such as "_","()", etc.
        iv) No duplicated variables or data.  
        
I made more in-depth comments throughout my code, but here is an outline of
the steps I took to clean and compile data set.



        1. Cleaned the data related to the feature variables.  I renamed the 
        variables given in the features_info.txt file according to tidy data
        principles.  The updated variable names are in the codebook. I checked
        see if there were any duplicated variables as well.  
        2. Cleaned the activities data file according to tidy data principles.
        3. Built the test and training data sets removing duplicated data.
        4. Merged the test and training data sets into a complete data set.
        5. Melted the data set to a narrow format.
