# HigherEducation

#### Introduction
Jamboree has helped thousands of students like you make it to top colleges abroad. Be it GMAT, GRE or SAT, their unique problem-solving methods ensure maximum scores with minimum effort.
They recently launched a feature where students/learners can come to their website and check their probability of getting into the IVY league college. This feature estimates the chances of graduate admission from an Indian perspective.

#### Problem Statement
Data analysis will help Jamboree in understanding what factors are important in graduate admissions and how these factors are interrelated among themselves. It will also help predict one's chances of admission given the rest of the variables.


### Inference:

* While university ranking, rating of SOP and LOR also have an impact on chances of admit, research is the only variable which doesn't have much of an impact.
* We can see from the scatterplot that the values of university ranking, SOP, LOR and research are not continuous so we can convert them into categorical variables.
* Chance of Admit shows strong correlation with GRE Score, TOEFL Score and CGPA.
* Research shows 0.5 correlation with GRE Score, CGPA as well as chance of admit implying students with research component have 50% chance of getting admission.
* Statement of purpose, SOP is correlated with LOR, Letter of Recommendations.
* GRE Score and TOEFL Score share a strong correlation meaning that students who are performing well in GRE are also doing doing well in TOEFL.
* CGPA shares a strong correlation with GRE as well as TOEFL Score implying that the student is good in his college subjects as well.
* Correlation matrix shows that exam scores (GRE, TOEFL) have a strong positive correlation with chance of admission and they are also strongly correlated with CGPA of the student.
* Almost all the variables excluding research have a very high level of collinearity. This was also observed from the correlation heat map which showed strong positive correlation between GRE, TOEFL scores and CGPA.
* 
* Mean of Residuals
It is clear from RMSE that Mean of Residuals is almost zero.

* Linearity of variables
It is quite clear from EDA that independent variables are linearly dependent on the target variables.
* While Linear Regression and Ridge regression have similar scores, Lasso regression has not performed well on both training and test data
* The distribution of target variable (chances of admit) is left-skewed
* Exam scores (CGPA/GRE/TOEFL) have a strong positive correlation with chance of admit. These variables are also highly correlated amongst themselves the categorical variables such as university ranking, research, quality of SOP and LOR also show an upward trend for chances of admit.
* From the model coefficients (weights), we can conclude that CGPA is the most significant predictor variable while SOP/University Rating are the least significant
* Both Linear Regression and Ridge Regression models, which are our best models, have captured upto 82% of the variance in the target variable (chance of admit). Due to high colinearity among the predictor variables, it is difficult to achieve better results.
* Other than multicolinearity, the predictor variables have met the conditions required for Linear Regression - mean of residuals is close to 0, linearity of variables, normality of residuals and homoscedasticity is established.
