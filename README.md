# Getting_and_Cleaning_Data

This repository contains the following files:
* README.md
* Codebook.md 
* run_analysis.R

1. After files downloaded I do the merge usind the command
mergedData <- rbind(train, test) 

2. With the mergind data, the script extracts the information of the mean and std. If you take a look at the features.txt file from the unzip folder, you will find what we need to extract. As we have also at the beginning of each line the subject and the analysis, we have to add 2 to each number to get the correct position. Now we have a data frame with only the selected columns. 

3. Reading the information from the .txt file, I have taken the description of each activity to rename the information on the dataframe. 
4. We make a loop to set the appropriate labels the data set with descriptive variable names. 
5. I have created a second, independent tidy data set with the average of each variable for each activity and each subject. I have not been able to do it on a loop, so it can be improved. 
 
Finally, I create to txt files, one with the dataframe and another one with the tidy_data
