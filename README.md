# homework-iv-IMLPye
# homework-iv-starter
Name: Ye Ouyang
ID: yo2258

There are two main files:
1)  .travis.yml: To configure the Travis and set the environment for test (Python 2.7, 3.4. 3.5 are used here)
2)   hw4_starter_notebook.ipynb: This file includes all codes for this homework


The following steps are included:
1)  Data Cleaning
      - Load the data
	  - Visualize the class distribution
	  - Clean up the target labels

	  
2)  Model 1
      - Use SGDClassifier to do the classification
	  - Use confusion matrix to report macro f1-score
      - The score is 0.53 which is better than 0.5 

	  
3)  Model 2
      - Improve the model by setting different parameters for three components in the Pipeline
	      - CountVectorizer
		  - TfidfTransformer
		  - SGDClassifier

	  
4)  Visualize Results
      - metrics.classification_report is used to do the visuluzaiton (classification results, confusion matrix, important features, example mistakes).

	  
5)  Clustering
      - Apply K-Means to the whole dataset to divide the data into different groups
	  - Set the number of cluster as 5 
	  - Relabel the datasets using the clustering results

	  
6)  Model 3
      - Use the clustered result to label dataset, and use the new label to do the classification
	  - Do classification again using the new dataset (relabelled data)
	  - Get accuary as 0.638 which is higher than 0.5
	  - Use assert to check the accuracy
	  - def test_accuracy():
			print (improvedModel())
			assert(improvedModel()>0.62)
	
	  
7)  Extra Credit
      - Use a word embedding representation like word2vec for step 3 and or step 6. 
      
      


