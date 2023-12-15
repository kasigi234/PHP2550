# Project Portfolio PHP2550
 These are projects we did during Fall 2023 semester in the Practical Data Analysis class (PHP2550). The projects covered the key main areas of data analysis. They included Exploratory Data Analysis (EDA), Regression Analysis and Simulation studies. In the first project we examined the relationship between prenatal and postnatal tobacco smoking on children's externalizing and self regulation outcomes, in the second project we built a predictive model for timing and indication for tracheostomy need in neonates with severe bronchopulmonary dysplasia (sBDP) while the last project focused on transporting a prediction model to a different population that the one it was developed and evaluated in (Non-simulated) and to a simulated population that mimics the target population based on available covariate information such as summary statistics. These projects were in collaboration with faculty from Brown University and were based on real data from their ongoing research studies. 

## Project 1: Examine the Relationship Between Pre/Postnatal Tobacco Exposure and Child Externalizing and Self Regulation Outcomes
Collaboration with Dr. Lauren Micalizzi

This project focused on investigating the impact of prenatal tobacco exposure on self-regulation, substance use, and externalizing behavior in children. Exposure to smoking during pregnancy and environmental tobacco smoke has shown to have profound effects on children, contributing to health issues and behavioral challenges. With a dataset comprising responses from a randomly selected sub-population of mothers and their adolescent children, aged 12-16 years, we aim to analyze the association between smoking during pregnancy (SDP) and environmental tobacco smoking (ETS) exposure and various outcomes in children. The exploratory analysis involved a thorough data pre-processing, including outlier removal, handling missing values, and data transformations. Our primary objectives was aimed at understanding the relationships between SDP(Smoking during pregnancy), ETS(Environmental Tobacco Smoking) exposure, and variables such as self-regulation, externalizing behavior, and substance use. 

## Project 2:Developing a Predictive Model for Timing and Indication for Tracheostomy Need in Neonates with Severe Bronchopulmonary Dysplasia
Collaboration with Dr. Chris Schimd

This project focused on developing regression models to predict the need for tracheostomy placement in neonates with severe bronchopulmonary dysplasia (sBPD). With extended ventilation becoming a common practice for infants surviving sBPD, the timing and criteria for tracheostomy placement remain unknown in pediatric care. We utilized the data from the BPD Collaborative Registry, respiratory parameters and demographic information collected at 36 and 44 weeks to build the models. These were the first models that considered respiratory parameters and postmenstrual ages, to provide models that could be used for clinical decision-making in the management of neonates with sBDP. In the analysis we used a trained generalized linear mixed-effects regression model, with Lasso being utilized for variable selection. The resulting prediction model demonstrates promising performance with an AUC of approximately 0.895 and 0.92 with the 36 and 44 weeks, respectively. Sensitivity (0.76), specificity (0.89), and overall accuracy (0.88) showed that we could rely on the 36 weeks model in identifying infants who may truly benefit from tracheostomy placement. 

![image](https://github.com/kasigi234/PHP2550/assets/132590202/3d834460-fb3e-47c1-88b5-4dcdd64f76f9)

## Transportability of Prediction Models in Diverse Populations (Simulated and Non-simulated Target Population)
Collaboration with Dr. Jon Steingrimsson of Brown University

In this project we were looking into how well prediction models work when we move them from one population where they were developed in to another different population. We also were interested in seeing how the same model will also perform in a simulated population that mimics the target population. For this project the target population that we were interested in did not have the outcome.  We used data from the Framingham Heart Study to predict the risk of heart disease in the NHANES group. Even though NHANES didn't have possess the outcome which was CVD. In order to transport the measures from our prediction model we ensured the positivity of the likelihood of being in the Framingham population for each covariate pattern in NHANES. To apply the prediction model and assess its performance in the target population, we employed inverse-odds weights to obtain brier score estimands, estimating the probability of belonging to the Framingham (source) population based on covariates statistics from the target population. We then used the Brier scores to obtain the evaluation metrics such as bias and standard errors.

The Inverse weights were obtained as below:
![image](https://github.com/kasigi234/PHP2550/assets/132590202/05d5cc94-34f2-4d5b-a14c-54b4ef5d391f)

and the Brier scores as below:
![image](https://github.com/kasigi234/PHP2550/assets/132590202/c9489795-8d44-44ad-8c64-9eeddac3b7ec)

In the evaluation phase, we used bias and standard errors to assess the performance of the transported prediction model, considering the Framingham data with outcome and the NHANES data without it.


we obtained the brier score estimator that was used as a measure of the models performance.based on the probability of being in the target population given the source population. to obtain the 




 We found that our prediction model worked okay, even when we didn't have all the data we wanted. This is important because it helps us make good decisions even when doing real-world tests is hard. Our study tells us how well our predictions work for heart disease in different groups of people. Check out what we did to see how you can use these predictions in your work.

In our study, we figured out a way to use just the important info to make predictions for the new group.


In the realm of predictive modeling, the challenge of assessing model performance across populations with varying levels of outcome information has prompted our investigation into the transportability of prediction models. With a focus on scenarios where detailed outcome data are lacking in the target population, we propose a novel methodology leveraging summary statistics for model transport. Drawing from the Framingham Heart Study and applying logistic risk models, our research predicts cardiovascular heart disease risk within the NHANES population. Through a transparent simulation study adhering to ADEMP principles, we extend prediction scores from Framingham to a simulated NHANES target population, showcasing the potential for predictive model applicability in diverse settings. Despite lacking long-term outcomes in NHANES, our comprehensive approach, including eligibility criteria alignment and inverse odds weighting, results in a predictive model exhibiting a moderate level of accuracy and good calibration. Simulations offer valuable insights into evidence-based decision-making, especially when real-world experiments are challenging. Our analysis sheds light on logistic regression model performance in predicting cardiovascular disease across different populations, providing a foundation for broader application and generalization. Explore our methodology and findings to enhance your understanding of predictive model transportability.




