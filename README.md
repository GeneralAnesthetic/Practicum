# Practicum
MSDS_692

Dementia defined: Impairment to memory and other cognitive abilities, which interferes with daily life. Dementia is caused by abnormal alterations in the brain (alz.org, n.d.).

I came across a dataset in Kaggle that applied Random Forest, Decision Tree and Gradient Boosting models to ‘Oasis_2’ Dementia data (Klymentiev, 2018). The set was obtained from an open-source platform that provides MRI, clinical assessment and questionnaire metrics from participants enrolled in brain imaging studies. One-hundred and fifty right-handed subjects, from ages sixty to ninety-six, were repeatedly scanned and asked to complete cognitive impairment assessments over the course of a year. The participants also submitted answers to questions relating to income and their level-of-education (oasis-brains, n.d.).  Classification with ML is fulfilling a growing need for medical diagnostic tools. And, it often either matches, or exceeds, clinician diagnostic performance (Martin, 2023).

The question I wanted to answer was: what other models could be applied to improve diagnosis classification accuracy? A previous effort on Kaggle produced an accuracy score of ~70% with a Random Forest model (Klymentiev, 2018). 

During this analysis, a Sklearn Pipeline was employed to decipher which model would result in the highest accuracy. Then, Grid Search and Cross Validation were applied to generate the best parameter values and to evaluate performance.  MLP ended up with the highest F1 and Accuracy Scores. MLP also generated the greatest percentages of ‘Area under the Curve’.
Multi-layer perceptrons (MLP) is a ‘feed-forward’ neural network. It uses linear regressions to compute weighted sums from input features influencing a main target. Similarly, MLP will weigh the input features against ‘hidden’ targets, or intermediary nodes/units. Next, weighted sums are calculated between these hidden units and the main target. And, more ‘layers’ of hidden units can be added to refine the decision boundary.  Finally, the weighted results, or coefficients, are subjected to a non-linear model (often rectifying nonlinearity, or ‘relu’, and tangens hyperbolicus, or ‘tanh’) that derives the segments of the classification boundary. ‘Relu’ discounts values below zero and ‘tanh’ pulls coefficients towards either ‘-1’, for low values, and ‘+1’, for the higher values. MLP is capable of producing accurate decision boundaries for classification and its hidden layers can accommodate large and small datasets by adjusting the number of hidden units and layers (Muller & Guido, 2016).  

<img src="C:/Users/Brain/Downloads/Picture4.png" class="img-responsive" alt=""> </div>
https://ibb.co/KFQYc5C
Multilayer Perceptron (Bento, 2021 Sept 21st, towardsdatascience.com)

MLP achieved the highest accuracy (83%).

AUC Accuracy (MLP):
<img src="C:/Users/Brain/Downloads/Picture5.png" class="img-responsive" alt=""> </div>
<img src="C:/Users/Brain/Downloads/Picture6.png" class="img-responsive" alt=""> </div>
<img src="C:/Users/Brain/Downloads/Picture6.png" class="img-responsive" alt=""> </div>
https://ibb.co/QnwwfZj


References:

Bento, Carolina (2021, Sept 21st). “Multilayer Perceptron Explained with a Real-Life Example and Python Code: Sentiment Analysis”. Towards Data Science. (n.d.). Retrieved March 7, 2024, from https://towardsdatascience.com/multilayer-perceptron-explained-with-a-real-life-example-and-python-code-sentiment-analysis-cb408ee93141

Klymentiev, Russian (2018, April 8th). “Dementia Prediction w/ Tree-based Models”. Kaggle. Retrieved March 2, 2024, from https://www.kaggle.com/code/ruslankl/dementia-prediction-w-tree-based-models

Martin, Sophie - (2023, Feb 3rd). Interpretable machine learning for dementia: A systematic review - .Alzheimer’s & Dementia - Wiley Online Library. DOI: https://doi.org/10.1002/alz.12948. Retrieved March 7, 2024, from https://alz-journals.onlinelibrary.wiley.com/doi/full/10.1002/alz.12948

OASIS Brains - Open Access Series of Imaging Studies. (n.d.). Retrieved March 1, 2024, from https://www.oasis-brains.org/

What is Dementia? Symptoms, Causes & Treatment. Alz.org. (n.d.). Retrieved March 2, 2024, from https://www.alz.org/alzheimers-dementia/what-is-dementia


Acknowledgement:
  When publishing findings that benefit from OASIS data, please include the following grant numbers in the acknowledgements section and in the associated Pubmed Central submission: P50 AG05681, P01 AG03991, R01 AG021910, P20 MH071616, U24 RR0213
You will acknowledge the use of OASIS data and data derived from OASIS data when publicly presenting any results or algorithms that benefited from their use. Papers, book chapters, books, posters, oral presentations, and all other printed and digital presentations of results derived from OASIS data should contain the following:

  Acknowledgments: "Data were provided by OASIS-2: Longitudinal: https://doi.org/10.1162/jocn.2009.21407

  OASIS-2: Longitudinal: Principal Investigators: D. Marcus, R, Buckner, J. Csernansky, J. Morris; P50 AG05681, P01 AG03991, P01 AG026276, R01 AG021910, P20 MH071616, U24 RR021382

