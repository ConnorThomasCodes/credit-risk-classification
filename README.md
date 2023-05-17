# credit-risk-classification
In this repository, we test and evaulate two different logistic regresion models for classifying healthy vs high-risk loan applications. The first model is constructed using the original dataset, which contains far more healthy applications compared to high-risk applications (75036 healthy vs 2500 high risk). The second model is constructed after using the RandomOverSampler module to increase the number of datapoints in each class to 112554 each.

* Original Data
  * Accuracy: 0.99
  * Precision: 0.87
  * Recall: 0.89
  * The original dataset, had a high overall accuracy, but this was skewed by the large number healthy applicants. While this model can easily classify those applicants as healthy, it has some struggles with classifying the high-risk applicants.

* RandomOverSampled Data
  * Accuracy: 0.99
  * Precision: 0.99
  * Recall: 0.99
  * After oversampling our original dataset to even out the categories, our model performs much better than it did originally, yielding precision and recall scores of 0.99 now.

After evaluating both logistic regression models, it seems clear that the RandomOverSampled model is the superior choice for our company. This model has a near-perfect precision and recall for predicting high-risk loan applications and is a significant improvement over the original model. It should be noted that with oversampling comes a risk of overfitting our dataset, but given the high costs that can result from bad loans, it is extremely important that we can classify these as best we can.
