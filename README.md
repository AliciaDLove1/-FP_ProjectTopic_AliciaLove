Interpretation: Logistic Regression

Overall performance
Logistic Regression achieved strong overall performance, with an accuracy of 0.815, meaning it correctly classified about 81% of the reviews. The weighted precision and F1 score also show that the model performs well on average across all classes, especially given the class imbalance in the dataset.

Strengths
•	Excellent performance on positive reviews, which make up the majority of the dataset. 
o	Precision: 0.81
o	Recall: 0.99
o	F1 score: 0.89
•	Handles high dimensional TF IDF features effectively.
•	Fast training time and stable performance.
•	Very high recall for positive sentiment means the model rarely misses positive reviews.

Weaknesses
•	Poor performance on neutral reviews (precision = 0.00, recall = 0.00).
The model struggles to distinguish neutral sentiment from positive or negative.
•	Low recall for negative reviews (0.26), meaning many negative reviews were misclassified.
•	Class imbalance heavily affects the model — the dominance of positive reviews biases predictions toward the positive class.
•	Short or ambiguous reviews are often misclassified.

Confusion matrix insights
•	Positive reviews: 
The model correctly predicted 779 out of 784 positive reviews — extremely strong performance.
•	Neutral reviews: 
Almost all neutral reviews were misclassified as positive or negative. This confirms the model cannot reliably detect neutral sentiment.
•	Negative reviews: 
Many negative reviews were predicted as positive (105 cases).
This shows the model struggles with subtle or polite negative wording.
•	The confusion matrix clearly reflects class imbalance, with the model leaning heavily toward predicting “positive.”
   
