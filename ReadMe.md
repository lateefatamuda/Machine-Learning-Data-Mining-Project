# Machine Learning & Data Mining Project
#### Using Python and Azure Machine Learning Studio

## Project Description
This project was carried out as part of the requirement for the completion of my Master's degree program in <b>Data Science</b> at the [University of Salford](https://www.salford.ac.uk/science-engineering-and-environment).


## Project Objective
The purpose of this project is to analyse different datasets using data mining techniques, draw conclusions based on the analysis, and finally to present the results in the form of a report.<br>

<a href="#dataset-description">Four datasets</a> were used in this project, they are:
- Maternal Health Risk Data
- Android Permissions Dataset
- Seeds Dataset
- Tourist Accommodation Reviews Data


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

1. Maternal Health Risk Data:

This dataset consists of 7 attributes and 1014 instances. These attributes are Age, Systolic Blood Pressure as SystolicBP, Diastolic BP as DiastolicBP, Blood Sugar as BS, Body Temperature as BodyTemp, HeartRate and RiskLevel. 

These attributes are the main risk factors for maternal mortality. The RiskLevel column is the class label or dependent variable for this dataset, while the other columns are the independent variables.

The aim is to apply *Classification algorithms* to create a model that can effectively predict maternal health risks. Successful prediction of women’s maternal health risks would be really helpful in reducing and ultimately ending preventable maternal mortality and promoting great health for women.

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

This dataset, `tourist_accommodation_reviews.csv`, was provided as part of the project brief and has been compressed, attached in this repository and can be found in the `tourist_accomodation_review_analysis` folder.

The dataset contains reviews gathered from hotels and restaurants visited by tourists. There are  5 attributes and 43741 instances in the file. The attributes are ID, Review Date, Location, Hotel/Restaurant name, and Review. 

The Review column contains the tourist reviews and would be mined for sentiment analysis, to get a better understanding of the feelings of the tourists about the hotels and restaurants they’ve visited and their needs.
This knowledge can be used to improve the services rendered and by extension customer experience.

For this analysis, the *Text Mining and Sentiment Analysis* was performed on the dataset.


## Analysis Performed
- Data exploration
- Data processing/cleaning
- Data visualization
- Classification
- Association Rules Mining
- Clustering
- Text Mining and Sentiment Analysis


## Result of the Analysis
There were six files produced from the analysis.

1. `decision_tree_classification.ipynb` : this file contains code from the implementation of the Decision Tree algorithm used for the classification of the Maternal Health Risk data.

2. `neural_network_classification.ipynb` : this file contains code from the application of the Artificial Neural Network on the Maternal Health Risk data, for classification purposes.

3. `association_rules_mining.ipynb` : this file contains code from the association rules analysis carried out on the Android Permissions Dataset for malware detection.

4. `clustering.ipynb` : shows the application of the K-Means and Hierarchical (Agglomerative) clustering algorithms on the Seeds Dataset.

5. `text_mining_sentiment_analysis.ipynb` : shows the analysis of the Tourist accommodation reviews data using text mining and sentiment analysis.

6. `report.pdf.zip` : this is a compressed/zipped PDF file that fully explains the processes, including the exploratory data analysis, data preparation and cleaning, the algorithms used and the evaluation of the results. 


## Evaluation of the Results

1. Maternal Health Data Classification

In this analysis two models were generated for the classification of this dataset, and we were able to determine that the Decision Tree model performed best with high accuracy and f1-score when compared to the Neural Network model.

The Decision Tree model would make more effective classification and predictions of the risk level, and would be appropriate for future deployment. With this model, we can guarantee that the maternal health risk of a woman would be predicted correctly 78% of the time.

2. Android Permissions vs Malware Vulnerability

The result of this analysis shows that there is about 47% chance that granting the `READ_PHONE_STATE` permission will make the device more vulnerbale to Malware attack. There is also high confidence of about 0.89 (i.e. 89% chance) that the device would be vulnerable to Malware when `READ_PHONE_STATE` and `RECEIVE_BOOT_COMPLETED` permissions are granted together.

The other permissions with a great chance of making an Android device susceptible to malicious attacks are `RECEIVE_BOOT_COMPLETED`, `INTERNET`, `WRITE_EXTERNAL_STORAGE`, `ACCESS_NETWORK_STATE`, and `ACCESS_WIFI_STATE`.

It was also observed that the above-listed Android permissions make up 80% of the top ten permissions granted by users. This means that these permissions have a significant impact on the vulnerability of devices, and users should be advised/warned about the risk of vulnerability to malicious attacks when they want to grant these permissions to websites or applications.

Another suggestion would be to advise Android device companies to update the operating systems of these devices regularly so as to reduce the vulnerabilities and protect users against these security risks.

3. Wheat seeds identification and Grouping

Based on the results of this analysis, we can conclude that the models are average performers, and of the two clustering algorithms used, the K-Means algorithm produced the clusters with better quality. 

For K-Means clustering, the DB Index is 0.928 and the Silhouette Coefficient is 0.401, which means that there is a high similarity between the data points in each cluster and there is an average level of difference between the clusters. For Hierarchical clustering, the DB Index is 0.940 and the Silhouette Coefficient is 0.397, which is similar to K-Means. Even though both clustering algorithms have high similarity measures, the dissimilarity measures were low.

We were able to successfully group the varieties of wheat into three clusters based on the properties of the kernel; however, some of the data points might be grouped wrongly.

4. Text mining and Sentiment analysis of Tourist accommodation reviews

From the result of the analysis, we were able to deduce that the sentiment is strong and positive. The reviews have more neutral words than positive or negative words combined, and positive words are also more than negative words, as the mean value for the positive score is 0.22, the negative score is about 0.029, and the neutral score is about 0.75.

Based on the number of negative reviews, `Da Mario hotel/restaurant` had the highest number of negative reviews, however, when compared to the total reviews, `Outdoor Restaurant` had the highest percentage of negative reviews, while `Thong Dee The Kathu Brasserie` had the lowest percentage of negative reviews.

To evaluate the words that were more frequently used in both positive and negative reviews, the `Da Mario hotel/restaurant` was chosen as it had the highest reviews. From the frequency plot and wordcloud visualization of the negative reviews, it was observed that some words like *service*, *terrible*, *price* and *never*, were mentioned several times and this should be explored as they can be a source of concern. For the positive reviews, words like *good*, *nice*, *great*, *best*, and *love* were frequently used.

With these results, we can infer that for the *30 hotels/restaurants* selected there were more positive words used in the reviews than negative words, which means more people liked and enjoyed the services at these hotels. For the `Da Mario hotel/restaurant`, the reviews show that they have great food, good service, and are loved by a lot of the tourists, however, a significant number of tourists still had terrible experiences and these are potential concerns that requires further investigation and need for improvement.


## Recommended Improvements
--


## Author

Lateefat Amuda


