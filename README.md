Multicollinearity Test
=
Methodology
--
- First in first, I did the autocorrelation analysis for the 95 raw variables and find out the highly correlation issue among them. Around 41 variables were dropped after test;
- After that, the new processed dataset can move on to the next tests. the autocorrelation issue is solved, the next challenge is the problem of multicollinearity. If a model has the problem of multicollinearity,
  it means that the bias of the model causes a lot of trouble for the accuracy of the model. So that, VIF and Farrar-Glauber Test provides a detection method for the problem; 
- In this case, VIF thresholds were set 10, the reason why I choose 10 as the threshold as the average VIF value for most variables is around 5, while a few discrete valus have unnormal vif values above 10, so, in this case I
  set the threshold at 10 in order to eliminate variables with severe covariance as well as to retain normal variables. The number of featurese remaining is 40;
- After did VIF test, Farrar-Glauber test was performed again for further feature screenig. It was found that the dataset could still be further optimised, the test showed that there were 21 variables with potential mulcollinearity
  issue, so if there 21 variables were removed, the dataset was left with 19 features for training and testing.

Dataset 
--
- The processed_train_final.csv is the dataset after did VIF test as well as autocorrelation test, the number of features is 40;
- The processed_train_final_v2_with_19_variables is the dataset after did VIF test, autocorrelation test and Farrar-Glauber test, the number of features is 19.
