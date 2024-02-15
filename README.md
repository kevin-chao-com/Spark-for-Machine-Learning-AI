# Spark-for-Machine-Learning-AI
This is the my lesson notes and exercises for a LinkedIn course, Spark-for-Machine-Learning-AI.

* Created by Kevin Chao (kevinchao@gmail.com)
* https://www.linkedin.com/in/kevin-chao-com/
* Latest updated on Feb 14, 2024

* The LinkedIn course:
	* Spark for Machine Learning & AI by Dan Sullivan:
	* https://www.linkedin.com/learning/spark-for-machine-learning-ai/welcome

1. Introduction to Spark and MLlib
2. Data Preparation and Transformation
	* Numeric:
		* MinMaxScaler
		* StandardScaler
		* Bucketizer
	* Text:
		* Tokenizer
		* HashingTF
3. Clustering
	* K-Mean
	* Hierarchical clustering with Bisecting K-means
4. Classification
	* Navie Bayes
	* Multilayer perceptron
	* Decision trees
5. Regression	
	* Linear regression
	* Decision tree regression
	* Gradient-boosted tree regression (requiredd significant time to build the model)
6. Recommendations
	* Collaborative Filtering
		* In Spark: Using Alternating Least Squares method
	* Content-Based Filtering
7. Tips for using Spark MLlib:
	* (1) Processing:
		* Collect, reformat, and transform data
			* Load data into Spark DataFrames
			* Include headers, or column names, in text file
			* Use **inferSchema=True**
			* Use **StringIndexer** to map from string to numeric indexes
	* (2) Model Building:
		* Apply machine learning algorithms to training data
			* Split data into trainging and test sets
			* Fit models using trainging data
			* Create predictions by applying a transform to the test data
	* (3) Validation:
		* Assess the quality of models built in step 2 
			* Use MLlib evaluators:
				* **MulticlassClassificationEvaluator**
				* **RegressionEvaluator**
			* Experimeny with multiple algorithms
			* Vary hyperparameters
	* Other suggestions:
		* (1) MLlibs Docs:
			* Detailed API documentation and examples
		* (2) Kaggle:
			* Data sets and articles
		* (3) AWS Data Sets:
			* Big data and public data sets