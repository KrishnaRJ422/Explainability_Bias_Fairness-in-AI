# Explainability_Bias_Fairness-in-AI
This is done as a part of my main project submission for MBA in Analytics programs.
This work focuses on bringing explainability to black box ML models, along with measuring fairness of the models and techniques to mitigate bias.
German credit score data set is considered as source for this study https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29 which is a binary label dataset that contains entries that contain customer financial and demographic information tagged with credit score(good/bad).
This work is inspired by the paper https://arxiv.org/pdf/2005.12379.pdf and https://arxiv.org/pdf/1811.11154.pdf being other reference.
This study is divided in to 3 parts:
 a) Exploratory data anaysis(EDA) through visualization, correalation analysis (klib library is used)
 b) Explainability (using SHAPley, ELI5)
 c) Fairness and bias mitigation (fairness metrics used are DI,SPD,EOD,AOD,ERD,CNT,TI; bias mitigation: pre-process(reweighing,DIR), in-process(AD,PRR) and post-process(EO,COD,ROC)).
 
 
REFERENCES:
https://shap.readthedocs.io/en/latest/
https://towardsdatascience.com/explain-any-models-with-the-shap-values-use-the-kernelexplainer-79de9464897a
https://medium.com/@tonyxu_71807/ensuring-fairness-and-explainability-in-credit-default-risk-modeling-shap-ibm-tool-kit-aix-360-bfc519c191bf?
https://towardsdatascience.com/explainable-ai-interpretability-of-machine-learning-models-412840d58f40 
https://towardsdatascience.com/shap-explained-the-way-i-wish-someone-explained-it-to-me-ab81cc69ef30
https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_classif.html
https://www.youtube.com/watch?v=81JSbXZ26Ls
https://www.kaggle.com/dansbecker/permutation-importance
