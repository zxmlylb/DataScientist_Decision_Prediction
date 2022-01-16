# DataScientist_Decision_Prediction
Statistical Learning Project LDA


Topic
In this assignment, we aim to apply the Linear Discriminant Analysis (LDA) method with given demographic, education, and professional experience, to predict whether data scientists will commit to job offers given by a company. Our model’s prediction could be useful to reduce the cost and time that the hiring company devote to job candidates. Further, our result could also help the company to improve their hiring advertisement strategy, so that they could reach their target candidates more effectively.

The Data Set
Our data set is obtained from a Big Data company that wants to hire data scientist who successfully passed some pre-hiring courses conducted by the company. The predictor provided by the data set includes the demographic backgrounds of the candidates like their city_development_index, gender; their previous professional experience like experience, previous company size and finally we are also given the education background like what type of degrees they obtained and major discipline of given candidates. We omit the observations that are incomplete or contains NA values in our predictors.

<img width="744" alt="Screen Shot 2022-01-15 at 11 12 53 PM" src="https://user-images.githubusercontent.com/93837295/149647026-db2cbfca-da0a-4c27-8c62-7cf92a8d9357.png">

<img width="815" alt="Screen Shot 2022-01-15 at 11 13 11 PM" src="https://user-images.githubusercontent.com/93837295/149647034-a24eda4c-6678-4a1d-8ced-e966160d7f84.png">


Model Evaluation
Given the available model evaluation parameters accuracy, sensitivity, specificity, false discovery rate, and false omission rate, we decide to adopt specificity and false discovery rate as the two metrics to help us decide an optimal threshold.

The two metrics that are considered important to our model in the real world are: specificity and false discovery rate. The specificity describes how well our model can identify the negative classifiers, in other words, how well our model is able to predict the withdrawal of a candidate. A higher specificity implies that the hiring company has a higher precision on predicting how unlikely a candidate would commit to the job offer, which helps reduce the unnecessary cost and time put towards such candidates. The second metrics - false positive rate describes how likely our model is going to make mistake in predicting the positive classifiers, in other words, how well our model is able to predict the candidates’ commitment to job offers. A lower false-positive rate indicates our model is making less false positives prediction and having higher precision in predicting the positive classifier. In visualize the relationship between the two metrics, we plot the two metrics on a dot graph with thresholds at an interval of 0.05. We find that as the threshold increases, there is a trade-off between specificity and false discovery rate. For example, when the threshold is at 0.1, the false discovery rate is at its lowest 0.33, where the

Specificity is at its lowest at 0.75. At this low threshold, the model can predict has the most accuracy in predicting if one candidate would commit to the job offer, but the worst accuracy in predicting if one would withdraw. On the other hand, a high threshold such as 0.9 boosts the specificity value of the model, but increases the false discovery rate, making it extremely inaccurate in predicting the commitment of a candidate, but highly accurate in predicting one’s withdrawal.

<img width="718" alt="Screen Shot 2022-01-15 at 11 13 59 PM" src="https://user-images.githubusercontent.com/93837295/149647052-621ec41d-bc14-4eab-9d04-c53ab1777955.png">
