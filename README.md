# Credit-Card-Fraud-Detection-Model
Using a Kaggle dataset and my experience from UCLA's Break Through Tech AI program, I created a logistic regression model to predict whether a credit card transaction is fraudulent. The link to the dataset can be found below. The Jupyter Notebook with the model is included in this repository.
https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023?resource=download

**Evaluation of the Dataset** <br/>
The dataset comprises credit card transactions by European cardholders in 2023. Sensitive information has been removed, and features V1-V28 are anonymized. The label 'class' indicates fraud (1) or not fraud (0). Despite anonymization making feature interpretation difficult, the dataset is clean with no null values and all features being numerical.

**Tools Used** <br/>
&emsp;Data Handling: Pandas, NumPy <br/>
&emsp;Visualization: Matplotlib, Seaborn <br/>
&emsp;Modeling and ML: Scikit-learn <br/>

**Choice of Model and Loss Function** <br/>
&emsp;Model: Logistic Regression (suitable for binary classification) <br/>
&emsp;Loss: Log loss (standard for classification models) <br/>

**Training of Model** <br/>
&emsp;Used train test split function  and LogisticRegression from Scikit-learn for model training.

**Evaluation of Model** <br/>
&emsp;Metrics: Log loss and accuracy. <br/>
&emsp;Hyperparameter Tuning: Tested various values of the hyperparameter 'C' (learning rate) and plotted log10(C) against log loss and
&emsp;accuracy to identify optimal values. Detailed findings are in the notebook. <br/>

Citation: 
@misc{nidula_elgiriyewithana_2023,
	title={Credit Card Fraud Detection Dataset 2023},
	url={https://www.kaggle.com/dsv/6492730},
	DOI={10.34740/KAGGLE/DSV/6492730},
	publisher={Kaggle},
	author={Nidula Elgiriyewithana},
	year={2023}
}
