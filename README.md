
<h1 style="color: blue;">Credit Card Fraud Detection CNN</h1>
<h2>In this project, I created a convolutional neural network to detect credit card fraud transactions.</h2>
<h3>Results</h3>
<img src = "https://i.imgur.com/bSVx13q.png"/><br>
<img src = "https://i.imgur.com/2xRMVRK.png"/><br>

<img src = "https://i.imgur.com/lvhPnWJ.png"/><br>

<img src = "https://i.imgur.com/UuMv24m.png"/>
<h3>Results Explanation</h3>

True Positive — when the model correctly identifies a fraudulent transaction <br>
True Negative — when the model correctly identifies a non-fraudulent transaction <br>
False Positive — when the model incorrectly labels a non-fraudulent transaction as fraudulent (think of your bank saying your everyday transaction could be fraudulent) <br> 
False Negative — when the model incorrectly labels a fraudulent transaction as non-fraudulent. As a banking customer, this is by far the worst thing that can happen <br>
If you have another look at the confusion matrix, it will make it easier to understand these terms

<h4>Results Table</h4>

| Metric                 | What it describes                                                    | Model Result | Notes                                                                                                                                                            |   |
|------------------------|----------------------------------------------------------------------|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|---|
| Recall                 | Percent of fraudulent transactions correctly identified by our model | 90%          |                                                                                                                                                                  |   |
| Accuracy               | Percent of *total* transactions correctly identified by our model    | 99.7%        | This statistic is somewhat misleading, given that the majority of transactions were negative                                                                     |   |
| Confusion Matrix       | Compares the models predictions to the actual class labels           | See Above    |                                                                                                                                                                  |   |
| AUC (Area Under Curve) | Calculates the total area under the ROC curve                        | 0.95         | Plots the true positive rate against the false positive rate. Good general measure for model classification effectiveness. A result above 0.9 is considered good |   |



As a bank, we want to do our best to not only maximize true positives, but also minimize false negatives. That's why <b>recall and the AUC are the most important results metrics</b>. Minimizing false negatives could possibly come at the cost of having more false positives, and this is actually a problem in data science known as the precision-recall tradeoff. I talked about it more in the notebook. If you're interested in learning more about it, as well as some other challenges that were solved during this process, check out my notebook :)<hr>

<h3>Applications of this CNN</h3>
This CNN creates significant value for any organization that deals with credit card transactions, particularly financial institutions. Since the start of working on this project, I envisioned myself working for a bank.
<hr>
<h3>Notebook Sections</h3>
0. Import and Settings<br>
1. Data Understanding<br>
2. DataFrame Preprocessing <br>
3. Feature Understanding<br>
4. CNN Classification Model<br>
5. Conclusion<br>
