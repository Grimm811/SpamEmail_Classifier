#Spam Email Classifier

##Overview

1. The project consists of two parts - Part 1 focusses on using a SVM to plot a non-linear boundary for a dataset; Part 2 focusses on using the SVM built to separate important emails from spam emails.  

2. The program uses an inbuilt SVMtrain function. I implemented the Gaussian kernel, and also selected the values of C and sigma that minimized error (see data3Params.m)

3. The preprocessing of emails included lower casing, stripping HTML, word stemming and normalizing URLS, email addresses, Numbers,     Dollars


4. After this each email is converted into a feature vector with length equal to the total number of words in the vocab list.
   The value of the i-th entry in the vector corresponds to whether the i-th word in the dictionary occurs in the email. 

##Acknowledgement

This project is part of an online Machine Learning course on Coursera. The flow of the program can be found in the comments of ex6 and ex6_spam.

##File Contents

###Part 1
1. ex6.m - Octave/MATLAB script for the first half of the exercise
2. ex6data1.mat, ex6data2.mat, exdata3.mat - Example Datasets
3. svmTrain.m - SVM training function
4. svmPredict.m - SVM prediction function
5. plotData.m - Plot 2D data
6. visualizeBoundaryLinear.m - Plot linear boundary
7. visualizeBoundary.m - Plot non-linear boundary
8. linearKernel.m - Linear kernel for SVM
9. gaussianKernel.m - Gaussian kernel for SVM
10. dataset3Params.m - Parameters to use for Dataset 3

###Part 2
1. ex6 spam.m - Octave/MATLAB script for the second half of the exercise
2. spamTrain.mat - Spam training set
3. spamTest.mat - Spam test set
4. emailSample1.txt, emailSample2.txt - Sample emails
5. spamSample1.txt, spamSample2.txt - Sample spams
6. vocab.txt - Vocabulary list
7. getVocabList.m - Load vocabulary list
8. porterStemmer.m - Stemming function
9. readFile.m - Reads a file into a character string
10. processEmail.m - Email preprocessing
11. emailFeatures.m - Feature extraction from emails


