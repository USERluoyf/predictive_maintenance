# 📊 predictive_maintenance 🛠️
<h2>This is a project as part of the Artificial Intelligence course of the degree in computer science for management at the university of bologna</h2>
<br>Specific analysis of the data collected by the sensors for the development of a Machine Learning application, which exploits the correlations discovered in the data set to provide a sufficiently valid and correct prediction regarding a probable failure of a machine.
<br>Dataset used: “AI4I Predictive Maintenance Dataset”
<br>Lnk: https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset
<br>The version of the dataset we used can be found in this github repository under the name "predictive_mainteniance.csv".

<br><h3>🎯 Objectives:</h3>
1. Refinement and pre-processing of the dataset used, so as to keep the data useful for the purpose and discard everything else.
2. Exploratory Data Analysis (EDA), i.e. an in-depth study of the dataset aimed at discovering its main characteristics and searching for possible patterns, using statistical analysis tools
3. Application of certain classification algorithms to see which one can do the job most accurately

<h3>Example of dataset samples after pre-processing </h3>
For information on the characteristics of the dataset please refer to the link at the top of the page

![exampledataser](https://github.com/michele-abruzzese/predictive_maintenance/blob/main/esempio%20dataset.png)

<h3>EDA (Exploratory Data Analysis)</h3>
The output shows the type of failure and its absolute frequency. A quick glance at the table below immediately shows that the number of failures detected is extremely low compared to the cases labelled 'No Failure'.

![frequency](https://github.com/michele-abruzzese/predictive_maintenance/blob/main/frequenza.png)

<h3>Correlation matricesg </h3>
In the first figure, we can observe the correlation between the various features, while in the second the correlation between the various types of failure. Analysing them, we can see, for example, a significant positive correlation of 0.88 between air temperature and process temperature, while there is a significant negative correlation of -0.88 between rotation speed and torque.

![correlation](https://github.com/michele-abruzzese/predictive_maintenance/blob/main/correlazione1.png)
![correlation](https://github.com/michele-abruzzese/predictive_maintenance/blob/main/correlazione2.png)

<h3>Data visualization </h3>
An imbalance was found in the dataset, as the number of machine failures was found to be 3.39%.

![sbilanciamento](https://github.com/michele-abruzzese/predictive_maintenance/blob/main/sbilanciamento.png)
![failures](https://github.com/michele-abruzzese/predictive_maintenance/blob/main/fallimenti.png)

<h3>Classification models </h3>

- Logistic regression
- KNN
- Support Vector Machine
- Random Forest
- Ada Boost
- XG Boost
- Naive Bayes
- Decision Tree Classifier
- Multi Layer Perceptron

<h3>Comparison of different configurations and solutions</h3>
The sorting yardsticks used were accuracy and running time, although the latter turns out to be quite irrelevant for ranking them. As can be seen from the image below, all the algorithms applied to the designated model turn out to have a more than remarkable accuracy, being for all between 96% and 98%. What varies considerably, however, is the execution time, ranging from the order of thousandths of a second for Naive Bayes to almost 10 seconds for the Multi Layer Perceptron.

![results](https://github.com/michele-abruzzese/predictive_maintenance/blob/main/results.png)

The 'XGB Classifier' algorithm returned an accuracy of 98% and an execution time of 0.4/0.5 s. For a more in-depth study, XGB data on the classification of records on the target attribute (precision, recall, f-1 score and support).

![xgb](https://github.com/michele-abruzzese/predictive_maintenance/blob/main/xgb.png)
