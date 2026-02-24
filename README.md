## What the Current Model Metrics Tell Us

**Accuracy:**  
The proportion of correctly classified instances. A high accuracy (like 1.0) means the model is performing very well on the test data.

**Precision:**  
For class 1 (default), it's the proportion of actual defaults among those predicted as default.  
For class 0 (no default), it's the proportion of actual non-defaults among those predicted as non-default.

**Recall:**  
For class 1 (default), it's the proportion of actual defaults that were correctly identified.  
For class 0, it's the proportion of actual non-defaults that were correctly identified.

**F1-Score:**  
The harmonic mean of precision and recall. It's a good metric for imbalanced datasets like this one, where default cases are much fewer.

**Confusion Matrix:**  
Shows the number of true positives, true negatives, false positives, and false negatives.

In our case, `[[255, 2], [35, 1]]` indicates:

- **255 True Negatives** – correctly predicted no default  
- **2 False Positives** – incorrectly predicted default when it was no default  
- **35 False Negatives** – incorrectly predicted no default when it was default  
- **1 True Positive** – correctly predicted default  

**ROC AUC Score:**  
Measures the model's ability to distinguish between classes across all possible classification thresholds. An AUC of 1.0 indicates a perfect classifier.
