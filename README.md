I have provided the screenshots of outputs and graphs in the output folder, the codes are provided in the ipynb format and the datasets are presnt in the data folder. 
Stepwise explanations are provided in the code file itself.

WHY CHOOSE RANDOM FOREST?
Based on the output provided, we have two classification models (likely two iterations of Logistic Regression), and the goal is to select the best model for predicting loan repayment behavior (specifically identifying potential defaulters and non-defaulters).
Model Evaluation Summary:
Model 1: LINEAR REGRESSION
Accuracy: 0.74
Precision (Class 0): 0.42
Recall (Class 0): 0.01
F1-Score (Class 0): 0.01
Precision (Class 1): 0.74
Recall (Class 1): 1.00
F1-Score (Class 1): 0.85
Model 2: RANDOM FOREST
Accuracy: 0.76
Precision (Class 0): 0.58
Recall (Class 0): 0.30
F1-Score (Class 0): 0.40
Precision (Class 1): 0.79
Recall (Class 1): 0.92
F1-Score (Class 1): 0.85


Analysis:
Model 1: This model shows a perfect recall for Class 1 (non-defaulters) (1.00), which means it classifies all defaulters correctly but has poor precision and recall for Class 0 (defaulters), leading to many false positives.
Model 2: This model strikes a better balance between precision and recall for both classes. While its accuracy is slightly higher (0.76 vs. 0.74), Model 2 performs better in terms of precision and recall for Class 0 (defaulters), which is essential for your goal of identifying loan defaulters.

So for the NBFC task of predicting loan repayment behavior, Model 2 seems like the better choice because it has a better balance between precision and recall, particularly for Class 0 (defaulters). It ensures fewer false positives (non-defaulters classified as defaulters) and a higher recall for Class 1, making it a more reliable model for detecting both defaulters and non-defaulters.


