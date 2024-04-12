Multicollinearity Test
=
Methodology
--
- Firstly, the challenge is the problem of multicollinearity. If a model has the problem of multicollinearity, it means that the bias of the model causes a lot of trouble for the accuracy of the model. So that, VIF and Farrar-Glauber   Test provides a detection method for the problem; 
- In this case, VIF thresholds were set 10, the reason why I choose 10 as the threshold as the average VIF value for most variables is around 5, while a few discrete valus have unnormal vif values above 10, so, in this case I
  set the threshold at 10 in order to eliminate variables with severe covariance as well as to retain normal variables. The number of featurese remaining is 51;

Dataset 
--
- The processed_train.csv is the dataset after did VIF test, the number of features is 51;
