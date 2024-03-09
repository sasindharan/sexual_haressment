# Sexual Harassment Detection Project

**Detailed Description of Machine Learning Algorithms:**
Provide a brief overview of each machine learning algorithm used in the project, including their strengths and weaknesses in the context of sexual harassment detection.
Explain how each algorithm is applied to the specific modality (text, images, audio) for harassment detection.
**Data Preprocessing Techniques:**
Describe the data preprocessing steps undertaken before training the machine learning models.
Include details about text preprocessing (e.g., tokenization, stopword removal, stemming/lemmatization), image preprocessing (e.g., resizing, normalization), and audio preprocessing (e.g., feature extraction, audio augmentation).
**Evaluation Metrics:**
Explain the evaluation metrics used to assess the performance of the trained models.
Provide definitions and interpretations of metrics such as accuracy, precision, recall, F1-score, ROC-AUC, and confusion matrix.
**Model Interpretability and Explainability:**
Discuss methods for interpreting and explaining the decisions made by the trained models, especially in sensitive domains like sexual harassment detection.
Mention techniques such as feature importance analysis, SHAP (SHapley Additive exPlanations) values, and LIME (Local Interpretable Model-agnostic Explanations).
**References:**
Include references to relevant research papers, articles, or documentation sources cited throughout the README file.
Provide links to external resources or libraries used in the project (e.g., TensorFlow, PyTorch, scikit-learn).
**Visualization and Demo:**
Include visualizations (e.g., graphs, charts) of model performance, dataset characteristics, or feature importance.
Provide a demo or example code snippets demonstrating how to use the trained models for harassment detection on sample data.


Single-Label Classification
The data for single-label classification is given in two columns, with the first column being the description of the incident and the second column being 1 if the category of sexual harassment is present and 0 if it is not.

Examples from Groping Binary Classification Dataset:

Description	Category
Was walking along crowded street, holding mums hand, when an elderly man groped butt, I turned to look at him and he looked away, and did it again after a while.I was 12 yrs old then.	1
This incident took place in the evening.I was in the metro when two guys started staring.	0
Catcalls and passing comments were two of the ghastly things the Delhi police at the International Airport put me and my friend through. It is appalling that the protectors and law enforcers at the airport can make someone so uncomfortable.	0
10% of each dataset was randomly selected and held-out for the test set. From the remaining training data, 10% was randomly selected and set aside for the development set.

Category	% Positive
Commenting	39.3%
Ogling	21.4%
Groping	30.1%
For each category, there are 7201 training samples, 990 development samples, and 1701 test samples.

Multi-Label Classification
The data for multi-label classification is given in four columns, with the first column being the description of the incident and the second, third, and fourth column being 1 if the category of sexual harassment is present and 0 if it is not.

Examples from Multi-Label Classification Dataset:

Description	Commenting	Ogling/Facial Expressions/Staring	Touching/Groping
Was walking along crowded street, holding mums hand, when an elderly man groped butt, I turned to look at h7m and he looked away, and did it again after a while.I was 12 yrs old then.	0	0	1
This incident took place in the evening.I was in the metro when two guys started staring.	0	1	0
Catcalls and passing comments were two of the ghastly things the Delhi police at the International Airport put me and my friend through. It is appalling that the protectors and law enforcers at the airport can make someone so uncomfortable.	1	1	0
10% of the dataset was randomly selected and held-out for the test set. From the remaining training data, 10% was randomly selected and set aside for the development set.

Commenting	Ogling	Groping	Examples in Dataset
1	1	1	351
1	1	0	819
1	0	1	459
0	1	1	201
1	0	0	2256
0	0	1	1966
0	1	0	743
0	0	0	3097
There are 7201 training samples, 990 development samples, and 1701 test samples.
