# Explainability_Bias_Fairness-in-AI (Responsible AI)
This work focuses on bringing explainability to black box ML models, along with measuring fairness of the models and techniques to mitigate bias.
German credit score data set is considered as source for this study https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29 which is a binary label dataset that contains entries that contain customer financial and demographic information tagged with credit score(good/bad).
Introduction to the bias and fairness:
https://krishnarj422.github.io/Explainability_Bias_Fairness-in-AI/Introduction_to_bias_fairness.html
This work is inspired by the paper https://arxiv.org/pdf/2005.12379.pdf and https://arxiv.org/pdf/1811.11154.pdf being other reference.
The protected attributes identified in this dataset are: Age, Gender.
This study is divided in to 5 parts:

 a) Exploratory data anaysis(EDA) through visualization, correalation analysis (klib library is used) 
 
 
 b) Explainability (using SHAPley, ELI5) on train data
 
 
 c) Fairness and bias mitigation (fairness metrics used are DI,SPD,EOD,AOD,ERD,CNT,TI; bias mitigation: pre-process(reweighing,DIR), in-process(AD,PRR) and post-    process(EO,COD,ROC)) along with explainability on test data on XGB,RF,KNN,LR,SVM using IBM's AIF360 toolkit in python.
 
 d) Senstivity Analysis using Google's What-If tool (WIT)
 
 e) Disparate Impact Analysis using Auto ML tool H2O.ai
 
 https://krishnarj422.github.io/Explainability_Bias_Fairness-in-AI/MAIN_PJT_EDA_UPD.html
 https://krishnarj422.github.io/Explainability_Bias_Fairness-in-AI/MAIN_PJT_RESP_AI_AGE_UPD.html
 https://krishnarj422.github.io/Explainability_Bias_Fairness-in-AI/MAIN_PJT_RESP_AI_GENDER_UPD.html

 It is found that the debaising has given better fairness performance in case of original data relative to oversampled data(ADASYN).
 

 Code for deployed hyper parameter tuned random forest model with protected attribute age is: https://github.com/KrishnaRJ422/German-Credit-Status. 
 
 Deployed application: https://credit-score-status.herokuapp.com/   ,   https://creditstatus.azurewebsites.net/
 
REFERENCES:
1. https://shap.readthedocs.io/en/latest/
2. https://towardsdatascience.com/explain-any-models-with-the-shap-values-use-the-kernelexplainer-79de9464897a
3. https://medium.com/@tonyxu_71807/ensuring-fairness-and-explainability-in-credit-default-risk-modeling-shap-ibm-tool-kit-aix-360-bfc519c191bf?
4. https://towardsdatascience.com/explainable-ai-interpretability-of-machine-learning-models-412840d58f40 
5. https://towardsdatascience.com/shap-explained-the-way-i-wish-someone-explained-it-to-me-ab81cc69ef30
6. https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_classif.html
7. https://www.youtube.com/watch?v=81JSbXZ26Ls
8. https://www.kaggle.com/dansbecker/permutation-importance
9. https://aif360.readthedocs.io/en/latest/modules/datasets.html
10. https://nbviewer.jupyter.org/github/IBM/AIF360/blob/master/examples/tutorial_credit_scoring.ipynb
11. https://aif360.mybluemix.net/
12. https://www.youtube.com/watch?v=jHojeFCc5HE
