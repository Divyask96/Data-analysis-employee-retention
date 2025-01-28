# Data-analysis-projects
This project is about solving a business problemfor the HR department of a company on how to recruit and retain the talent. HR team wants to incentivize employees to retain them. But the question is who should they be incentivizing with limited budget?HR management wants to know the likelihood of employees who will stay with the company, employees who will leave despite being rewarded, and employees who will fall somewhere in between, so that they can offer a bonus to secure them.

The data set has 4635 observations with 9 different variables including education, joining year, payment tier, experience and some more. The variable summary helped us in identifying the null values in input variables and target variable in detail. We performed data visualization comparing different variables and discovered that female employees, employees with master's degrees, employees with Payment Tier 2, and employees from Pune City are a few observations in which we see a higher probability of employees leaving the company than staying with the company. After some general observations and visualizations, the Chi-Square Statistics, often known as the Goodness of Fit statistic, helped us in identifying the highly significant variables such as Payment Tier, Gender, City, Joining Year, Education, and Ever Benched. 

The datset was then partitioned into  Train (80%) and Test (20%). The probability of leaving the company is classified as follows:
0 to 0.3 – Indicates the probability of employees not leaving the company. There is no need to incentivize because they won’t leave the company.
0.3 to 0.65 – Indicates the probability of employees that are uncertain (Undecided) whether to leave or stay with the company. These employees need to be incentivized to obtain maximum retention.
0.65 to 1.0 – Indicates the probability of employees who are leaving the company, there is not need to incentivize because they will leave the company even if they are incentivized.

To see the predictions, we ran out data through SAS Miner using Logistic Regression, Decision Trees, and Neural Networks (Optional) Models. Using neural networks, the missclassification rate on test data is 0.16, with decision trees we acheived an accuracy of 84.17%, precision of 91.77%, recall of 59.29%, and with logistic regression, we identified the accuracy to be 73.79% and precision to be 69.92%. The confusion matrix allowed us to have a detailed view of model's classification results. True positives (908), True negatives (2277), False positives (164), False negatives (372). We then compared these models and thus identified that decision trees is the best model for this prediction.
