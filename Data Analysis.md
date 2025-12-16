The model trained with all the data showed robust performance in predicting the final state of the projects.
LightGBM, assessed by five-fold stratified cross-validation, achieved a mean ROC-AUC of 0.800 ±0.001, indicating good discriminatory ability between successful and unsuccessful projects (Figure 1).
These values demonstrate that the model was able to stably capture relevant patterns in the variables related to the breeder.

<img width="1770" height="1170" alt="roc modelo geral" src="https://github.com/user-attachments/assets/d105961d-c2fe-4276-9ff1-c13c3bbf689f" />
Figure 1. ROC curve of the trained LightGBM model with stratified cross-validation (k = 5).
True positives are successfully funded Kickstarter projects and correctly predicted as such, while false positives are projects that did not reach their goal but were mistakenly classified as successful.
