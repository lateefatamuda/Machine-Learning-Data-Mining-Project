# Machine Learning & Data Mining Projects 
#### Using Python and Azure Machine Learning Studio

## Project Description
This project was carried out as part of the requirement for the completion of my Master's degree program in <b>Data Science</b> at the [University of Salford](https://www.salford.ac.uk/science-engineering-and-environment).


## Project Objective
The purpose of this project is to analyze different datasets using data mining techniques, draw conclusions based on the analysis, and finally to present the results in the form of a report.<br>
Four datasets were used in this project, they are:
- Maternal Health Risk data
- Android Permissions Dataset
- Seeds Dataset
- Tourist accommodation reviews data.



## Technologies and Platforms Used
Below are some of the technologies and platforms used in this project:
* Python
* Pandas
* Matplotlib
* Seaborn
* Jupyter
* Google Colab
* Azure Machine Learning Studio



## Dataset Description

1. Maternal Health Risk data:

This dataset consists of 7 attributes and 1014 instances. These attributes are Age, Systolic Blood Pressure as SystolicBP, Diastolic BP as DiastolicBP, Blood Sugar as BS, Body Temperature as BodyTemp, HeartRate and RiskLevel. 

These attributes are the main risk factors for maternal mortality. The RiskLevel column is the class label or dependent variable for this dataset, while the other columns are the independent variables.

The aim is to apply *Classification algorithms* to create a model that can predict maternal health risks. Successful prediction of women’s maternal health risks would be really helpful in reducing and ultimately ending preventable maternal mortality and promoting great health for women.

Source of the data: [UCI/MaternalHealthRiskDataset](https://archive.ics.uci.edu/dataset/863/maternal+health+risk)


2. Android Permissions Dataset:

This dataset contains 87 attributes and 29333 instances, 86 of these attributes are permissions and the last attribute is the Result. The Result column is like a label, it signifies the presence or absence of malware in the device, it was renamed to Malware to make the data and analysis easier to understand.

The data is made up of Categorical variables which are stored in a numerical form of ones and zeros, to denote 'Yes' and 'No'. This dataset was used for *Association Rules Mining*, to uncover the relationship between Android permissions and the presence of malware in a device.

With this analysis, we will answer the question; *Which permissions would make the device vulnerable to malicious attacks if granted?*

Source of the data: [UCI/AndroidPermissionDataset](https://archive.ics.uci.edu/dataset/722/naticusdroid+android+permissions+dataset)


3. Seeds Dataset:

This dataset consists of 7 attributes and 210 instances. The attributes include Area A, Perimeter P, compactness C, Length, and Width of the kernel, as well as the Asymmetry coefficient and the Length of the kernel groove. The data is made up of continuous numerical variables.

The instances contain randomly selected observations of kernels belonging to three different varieties of wheat: Kama, Rosa, and Canadian, with 70 observations each.

*Clustering algorithms* were applied to this dataset, for efficiet identification and grouping of varieties of wheat produces, based on the type of kernel properties.

Source of the data: [UCI/SeedsDataset](https://archive.ics.uci.edu/dataset/236/seeds)


4. Tourist accommodation reviews data:

This dataset, `tourist_accommodation_reviews.csv`, was provided as part of the project brief. The dataset contains reviews gathered from hotels and restaurants visited by tourists. There are  5 attributes and 43741 instances in the file. The attributes are ID, Review Date, Location, Hotel/Restaurant name, and Review. 

The Review column contains the tourist reviews and would be mined for sentiment analysis, to understand the emotions of tourists about the hostels and restaurants they’ve visited. This was the dataset used for the Text Mining and Sentiment Analysis task.



## Tasks Performed
- Data exploration
- Data processing/cleaning
- Data visualization
- Classification
- Association Rules Mining
- Clustering
- Text Mining and Sentiment Analysis



## Result of the Analysis
There were six files produced from the analysis.

1. Decision_Tree.ipynb : this file contains code from the implementation of the Decision Tree algorithm used for the classification of the Maternal Health Risk data.

2. Neural_Network.ipynb : this file contains code from the application of the Artificial Neural Network on the Maternal Health Risk data, for classification purposes.

3. Association_Rules.ipynb : this file contains code from the association rules analysis carried out on the Android Permissions Dataset for malware detection.

4. Clustering.ipynb : shows the application of the K-Means and Hierarchical (Agglomerative) clustering algorithms on the Seeds Dataset.

5. Text_Mining&Sentiment_Analysis.ipynb : shows the analysis of the Tourist accommodation reviews data using text mining and sentiment analysis.

6. Report.pdf : this is a PDF file that fully explains the experimental process, including the exploratory data analysis, data preparation and cleaning, the algorithms used and the evaluation of the results. 

## Author

Lateefat Amuda


