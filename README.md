# Credit-Card-Fraud-Detection-Model
Using a Kaggle dataset and my experience from participation in UCLA's Break Through Tech AI program, I created a logistic regression model based on the cited dataset to predict whether a credit card transaction was fraud or not. 
The dataset used can be found here: https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023?resource=download

**Evaluation of the Dataset**
According to the Kaggle description, this dataset originates from the credit card transactions made by European cardholders in 2023, fairly recent. To protect the privacy of the cardholders, the sensitive information has been removed. Features V1-V28 have been anonymized to protect user privacy. These features represent different transaction attributes (time, location, etc.). Other features include id and amount. The label was known as 'class' or a binary value to indicate whether fraud or not. While the anonymization of the features is beneficial to user privacy, it also proved to be a drawback. It made it difficult to see what features went on into predicting the label. Furthermore if correlations were studied, it would just tell us which column had which correlation rather than what kind of data that column held. Yet, all in all, user privacy/data privacy is an important aspect to consider when collecting data. 

**Tools Used**
Jupyter Notebook was used for the data cleaning, data visualization, modeling, and machine learning. Pandas and NumPy were used to import, view, and clean the data. Matplotlib and Seaborn were used to help visualize training loss and accuracy scores of the logistic regression model. 

**Choice of Model and Loss Function**
Logistic regression is a type of linear model. It is an effective machine learning model to use in cases of classification, specifically binary classification. This makes it an optimal choice for our machine learning problem as the label being predicted is fraud (1) or not fraud (0). In cases of a classification model, it is standard to use a log loss function, whereas a regression model it may be more useful to use a mean squared error function. 

**Training of Model**
Used train test split function provided by and LogisticRegression() model object provided by sklearn to do heavy lifting. 

**Evaluation of Model**
A logistic regression model offers a log loss function to aid in the evaluation of the model. A logistic regression model has the hyperparameter 'C', otherwise known as the learning rate. Multiple values of C were tested. For each, the log loss and accuracy score was recorded. Graphs were then plotted of the log10(C) and the log loss as well as the accuracy score to observe which values of C optimized the model. Findings can be found within markdown cells in the notebook. In a more complex model, it may be useful to create our own gradient descent function to find the best learning rate. In this simple case, testing arbitrary values seemed to yield low log loss and high accuracy. To fine tune a model further, it can be useful to use gradient desent in logistic regression training. 


Citation: 
@misc{nidula_elgiriyewithana_2023,
	title={Credit Card Fraud Detection Dataset 2023},
	url={https://www.kaggle.com/dsv/6492730},
	DOI={10.34740/KAGGLE/DSV/6492730},
	publisher={Kaggle},
	author={Nidula Elgiriyewithana},
	year={2023}
}
