# Project Portfolio PHP2550
 These are projects we did during Fall 2023 semester in the Practical Data Analysis class (PHP2550). The projects covered the key main areas of data analysis. They included Exploratory Data Analysis (EDA), Regression Analysis and Simulation studies. In the first project we examined the relationship between prenatal and postnatal tobacco smoking on children's externalizing and self regulation outcomes, in the second project we built a predictive model for timing and indication for tracheostomy need in neonates with severe bronchopulmonary dysplasia (sBDP) while the last project focused on transporting a prediction model to a different population that the one it was developed and evaluated in (Non-simulated) and to a simulated population that mimics the target population based on available covariate information such as summary statistics. These projects were in collaboration with faculty from Brown University and were based on real data from their ongoing research studies. 

## Project 1: Examine the Relationship Between Pre/Postnatal Tobacco Exposure and Child Externalizing and Self Regulation Outcomes
Collaboration with Dr. Lauren Micalizzi

This project focused on investigating the impact of prenatal tobacco exposure on self-regulation, substance use, and externalizing behavior in children. Exposure to smoking during pregnancy and environmental tobacco smoke has shown to have profound effects on children, contributing to health issues and behavioral challenges. With a dataset comprising responses from a randomly selected sub-population of mothers and their adolescent children, aged 12-16 years, we aim to analyze the association between smoking during pregnancy (SDP) and environmental tobacco smoking (ETS) exposure and various outcomes in children. The exploratory analysis involved a thorough data pre-processing, including outlier removal, handling missing values, and data transformations. Our primary objectives was aimed at understanding the relationships between SDP(Smoking during pregnancy), ETS(Environmental Tobacco Smoking) exposure, and variables such as self-regulation, externalizing behavior, and substance use. 

## Project 2:Developing a Predictive Model for Timing and Indication for Tracheostomy Need in Neonates with Severe Bronchopulmonary Dysplasia
Collaboration with Dr. Chris Schimd

This project focused on developing regression models to predict the need for tracheostomy placement in neonates with severe bronchopulmonary dysplasia (sBPD). With extended ventilation becoming a common practice for infants surviving sBPD, the timing and criteria for tracheostomy placement remain unknown in pediatric care. We utilized the data from the BPD Collaborative Registry, respiratory parameters and demographic information collected at 36 and 44 weeks to build the models. These were the first models that considered respiratory parameters and postmenstrual ages, to provide models that could be used for clinical decision-making in the management of neonates with sBDP. In the analysis we used a trained generalized linear mixed-effects regression model, with Lasso being utilized for variable selection. The resulting prediction model demonstrates promising performance with an AUC of approximately 0.895 and 0.92 with the 36 and 44 weeks, respectively. Sensitivity (0.76), specificity (0.89), and overall accuracy (0.88) showed that we could rely on the 36 weeks model in identifying infants who may truly benefit from tracheostomy placement. 

![image](https://github.com/kasigi234/PHP2550/assets/132590202/3d834460-fb3e-47c1-88b5-4dcdd64f76f9)

![image](https://github.com/kasigi234/PHP2550/assets/132590202/39cb71da-6c98-4897-837c-e6d51f2f1506)




