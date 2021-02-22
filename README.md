# LeoYin-Soft-Clustering-of-Functional-Point-Processes
Research Project

Project Status: working;

Introduction to the project "Semi-parametric Learning of Functional Point Process",

key words: Functional PCA; EM algorithm; GPU; array programming;
 
 ## Brief Introduction to the Project
 ### Code Description
 This code shows a GPU implementation of a joint model for temporal point processes and time-to-event outcomes through Pytorch. 
 
 ### Project Description
 An important goal in studying human activity patterns is to identify user groups displaying similar behavioral patterns. We will propose a method to cluster the credit card customers into sub-populations in terms of their credit card transaction records; Also, the proposed method can be applied to study other human acitivities, such as the posting and reposting acitivities on Twitter, buying activities of stock investors;
 
 
 ### Data Description
We investigated credit card transaction data set, which was collected by Worldline and the Machine Learning Group (http://mlg.ulb.ac.be) of ULB (Université Libre de Bruxelles) and can be accessed via https://www.kaggle.com/arslanali4343/credit-card-cheating-detection-cccd. The data set contains 641,914 transaction records of 5,000 European credit card customers during the period covering January 1 to December 31, 2016. There is a large variation in the
frequencies across accounts where the total number of annual transactions ranges from 0 to 10,034.
 
 
 ### Methodology
 Proposed hierarchical mixtured Poisson model, to describe the clustered human acitivties;
 
 Developed a semi-parametric EM algorithm, combined with functional PCA, which is far more computationally efficient and requires less storage complexity than the traditional EM algorithm while solving complicated mixture models;
 
 Accelerated the proposed algorithm by array programming and coded with Pytorch, so that GPU acceleration could be implemented in this project;
 
 
 ### Results
 The credit card customers are clustered into 6 groups, and the Figure below shows the estimated intensity functions within each cluster;
 
 ![image](Figures/ESL.png)
