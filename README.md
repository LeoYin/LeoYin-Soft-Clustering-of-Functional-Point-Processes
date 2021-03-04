# LeoYin-Soft-Clustering-of-Functional-Point-Processes
Research Project

Project Status: working;

Introduction to the project "Semi-parametric Learning of Functional Point Process",

key words: Functional PCA; EM algorithm; GPU; array programming;
 
 ## Brief Introduction to the Project
 ### Code Description
 This code shows a GPU implementation of a joint model for temporal point processes and time-to-event outcomes through Pytorch. 
 
 ### Project Description
 An important goal in studying human activity patterns is to identify user groups displaying similar behavioral patterns. One can further look into each cluster to better understand the underlying cause for certain activity patterns and to make some necessary adjustments (e.g. behavioral interventions). The goal of this project is to develop a unified approach to model human activity patterns and simultaneously form user clusters accordingly.
 
 The figures below show the time stamps for Twitter users in a window of 30 consecutive days. The blue points indicate the posting acitivities and the black indicate the reposting activities. All the users clearly seem to have strong clustered patterns. However, these posting patterns differ significantly in many ways, such as posting frequencies, percentages of original posts and reposts, and strengths of clustering. It is of interest to characterize these activity patterns and quantify their differences. We also want to know more specific questions including, (a) what the distribution of posting in one day; (2) how many posts would a user generate during each use? (c) how user-related characteristics were related to the posting and reposting patterns? (d) What are correlations among the posting activities of different days and the correlations between posting and reposting activities;
 
![image](Figures/Data.png) 
 
 
 ### Data Description
The team has access to data from 54,773 followers of a public Twitter account during the period of Nov. 30th, 2011 to Nov. 16th, 2013. In addition to posting times, user-related information such as the numbers of followers and followees of the account are also available.
 
 
 ### Methodology
 Proposed hierarchical mixtured Poisson model, to describe the clustered human acitivties;
 
 Developed a semi-parametric EM algorithm, combined with functional PCA, which is far more computationally efficient and requires less storage complexity than the traditional EM algorithm while solving complicated mixture models;
 
 Accelerated the proposed algorithm by array programming and coded with Pytorch, so that GPU acceleration could be implemented in this project;
 
 
 ### Results
 The Twitter users are clustered into 6 groups, and the Figure below shows the estimated intensity functions within each cluster;
 
 ![image](Figures/ESL.png)
