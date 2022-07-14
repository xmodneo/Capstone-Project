# Social network Graph Link Prediction 

Problem statement:<br>
Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph)<br>
<br>
Data Overview:<br>
Data is taken from the facebook’s recruiting competition hosted at Kaggle in 2012. It has 2 columns, a source_node (int64) and destination_node(int64)<br>
<br>
Mapping the problem into supervised learning problem:<br>
We first generate training samples of bad and good links from the given directed graph. Then we got some feature for each link, I.e total number of followers, total followee, page rank, Katz score Adar index hit score and svd features of adjancy matrix and some weight features etc. We the train two separate machine learning models on these features to get the best performing model.<br>
<br>
Performance metric for supervised learning:<br>
Both precision and recall are important so F1 score is good choice and plotted the Confusion matrix.<br>
<br>
To run the sample code,
<br>• Clone the repository: git
<br>• Raw data is already present in zip form: Run the 0_utilities.ipynb to unzip data
<br>• The data folder contains all the processed files containing all the necessary features for model
training. Trained models are also present in data folder.
<br>• Make sure to have all the required libraries present in lib.txt
<br>• First Time Run: Run the code files in the following sequence: 1_EDA, 2_SplitData,
3_Data_Featurization,4_PredictionModel_RandomForest, 5_Prediction Model_XGBoost<br>
<br>References:
<br>Data: https://www.kaggle.com/c/FacebookRecruiting
<br>Problem approach:<br> https://www.cs.cornell.edu/home/kleinber/link-pred.pdf<br> https://www3.nd.edu/~dial/publications/lichtenwalter2010new.pdf <br>https://www.youtube.com/watch?v=2M77Hgy17cg
<br>https://kaggle2.blob.core.windows.net/forum-message_attachments/2594/supervised_link_prediction.pdf
