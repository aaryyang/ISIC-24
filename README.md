**About the code:** 
It was borrowed from Master "Vyacheslav Bolotin" involving data from competition itself and several datasets including tf_efficientnetv2_b0 isic 2024 cancer specific, ISIC 2024 Effnetb0 LB 0.151, ISIC 2024 ImageNet Gen 2 Output, ISIC 2024 LGBM+ImageNet (OOF Pred Train) Output, ISIC 2024 Multifold V2 (offsite train), ISIC 2024 Multifold V3 (offsite train), Imagenet .143LB from isic-2024-imagenet-model-a, ISIC 2024 - Skin Cancer Detection with 3D-TBP, ISIC 2024 Tabular Feature Generation, ISIC 2024 ImageNet / LR Ramp + Target Mods.

**Goals:**
To identify cancers among skin lesions cropped from 3D total body photographs.
The image quality resembles close-up smartphone photos, which are regularly submitted for telehealth purposes.
Binary classification algorithm could be used in settings without access to specialized care and improve triage for early skin cancer detection.

**Evaluation:**
Primary Scoring Metric
Submissions were evaluated on partial area under the ROC curve (pAUC) above 80% true positive rate (TPR) for binary classification of malignant examples.

**Submission File:**
For each image (isic_id) in the test set,we predicted the probability (target) that the lesion is malignant.

**Final Results:**
The code mentioned has scored 0.185 in public leaderboard and 0.169[silver medal solution] in private leaderboard.

**Learnings:**
Learned various parameters of XGBoost,LightBoost and CatBoost. Also, on how noise plays a role in overfitting.
