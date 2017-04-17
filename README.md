# homework-iv-IMLPye
# homework-iv-starter
Name: Ye Ouyang
ID: yo2258

There are two main files:
1)  .travis.yml: To configure the Travis and set the environment for test
2)  hw4_starter_notebook.ipynb: The file containing the codes


The following steps are included:
1)  Data Cleaning
      - Load the data
	  - Visualize the class distribution
	  - Clean up the target labels.

	  
2)  Model 1
      - Use SGDClassifier to do classification
	  - Use confusion matrix to report macro f1-score
      - The score is 0.53 which is better than 0.5 

	  
3)  Model 2
      - Improve the model by setting different parameters for
	      - CountVectorizer
		  - TfidfTransformer
		  - SGDClassifier

	  
4)  Visualize Results
      - metrics.classification_report is used to do the visuluzaiton (classification results, confusion matrix, important features, example mistakes).

	  
5)  Clustering
      - Apply K-Means to the whole dataset
	  - Set the number of cluster as 5 

	  
6)  Model 3
      - Use the clustered result to label dataset
	  - Do classification again using the new dataset (relabelled data)
	  - Get accuary as 0.638 which is higher than 0.5


	  
7)  Extra Credit
      - Use a word embedding representation like word2vec for step 3 and or step 6. 
      
      
Use travis to run your notebook and add an “assert” statement inside the notebook that ensures the outcome is the actual error you report for each of the tasks.
(Say, if you claim your algorithm is 90% accurate, add an assert statement that score returned by your model is at least 90%).
Travis will simply run the notebook and check that it ran without errors.

We recommend that you fork the homework repository and run Travis on your own repository - this way you don’t have to wait for other students submissions to finish on travis.

