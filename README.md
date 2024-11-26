<div id="header" align="center">

# Drug Information & Side-Effects AI Model   <img src="https://media.giphy.com/media/5xtDaryFk1nV0vqfnws/giphy.gif?cid=ecf05e47sfjsrzdh193d20b012pew9qift150y4kkey5f82q&ep=v1_gifs_search&rid=giphy.gif&ct=g" width="30px"/>
</h1>
</div>

*Project Overview*

This project aims to build a machine learning model capable of identifying drugs from user input. Downloading the CSV file of drug information from https://www.kaggle.com/datasets/ahmedshahriarsakib/assorted-medicine-dataset-of-bangladesh?select=generic.csv, the dataframe is cleaned, split, trained using Gradient Boost Regression to classify drugs based on the user's description or name of the drug, aiding in quick and accurate identification. The resulting output would be medical information about the drug requested and the possible side-effects.

*Motivation*

With the rise in prescription medication usage, quick and reliable drug identification can be crucial for safety, especially in healthcare environments. his tool aims to assist in identifying drugs with accuracy and efficiency, potentially reducing errors, saving time and providing crucial information

*Features:*

	•	Comprehensive Dataset: CSV file from https://www.kaggle.com/datasets/ahmedshahriarsakib/assorted-medicine-dataset-of-bangladesh?select=generic.csv
	•	Potential for Real-World Application: A tool that could be used in healthcare, pharmacies, or for individual safety purposes.
	•	Drug Identification: Classifies drugs using advanced machine learning techniques.
	•	
	

*Getting Started:*

Installation


*Prerequisites:*

	•	Python 3.8+
	•	Required libraries: pandas, numpy, torch, and transformers
	•	Google Drive (for accessing the dataset)
 	•

*Steps:*

	•	Access (https://www.kaggle.com/datasets/ahmedshahriarsakib/assorted-medicine-dataset-of-bangladesh?select=generic.csv) and aquire the CSV file
	•	Create a dataframe of the drug description and other features
	•	Data Preprocessing (clean, categorize, and split)
	•	Train using Gradient Boost Regression, cross-validate, optimize the model by using HyperParameter Tuning (GridSearchCV and RandomizedSearchCV) to improve accuracy
	•	Test user input and provide output using a Gradio Interface

 *Dataset*

 	•	Dataset file generic.csv
	•	1,711 entries of drug information
	•	22 features

*Model Architecture:*

	Our model is 
 	Gradient Boost Regression 
		calculates the difference between the current prediction and the known correct target value.

  	Sentence Transformer
		create high-quality embeddings for sentences and text passages. 

*Model Metrics:*

Initial Regression Metrics:

Mean Squared Error (MSE): 0.11385 Mean Absolute Error (MAE): 0.16358 R-squared (R²): 0.01664 Interpretation: MSE and MAE are both low, suggesting that the model predictions are reasonably close to the actual values. An R-squared value of 0.0164 indicates that the model explains only about 1.64% of the variance in the target variable. This suggests a weak model performance, and I may need to explore feature engineering, hyperparameter tuning, or using different model architectures to improve my results.

Hyperparameter Tuning:

 Explanation: GridSearchCV: This class performs exhaustive search over specified parameter values for an estimator. The best parameters are determined based on the cross-validated performance. Parameter Grid: This grid specifies the values for different hyperparameters that I want to test. Model Training and Evaluation: After finding the best parameters, I will train the model again and evaluate its performance.

RandomizedSearchCV: This class performs a random search over parameter values instead of an exhaustive search, which can significantly reduce the computation time. n_iter: This parameter specifies the number of different combinations to try. Adjust this number based on time constraints.

The output from the RandomizedSearchCV indicates that the hyperparameter tuning was successful. Here’s a summary of the results:

Best Parameters: n_estimators: 200 min_samples_split: 3 min_samples_leaf: 1 max_depth: 3 learning_rate: 0.01 Model Performance: Best Mean Squared Error from CV: 0.14372 Mean Squared Error (Best Model - Random Search): 0.10960 Mean Absolute Error (Best Model - Random Search): 0.14175 R-squared (Best Model - Random Search): 0.05335 Interpretation: The Mean Squared Error (MSE) has slightly improved with the best model parameters found through random search. The R-squared value is still low (0.05335), indicating that the model explains only about 5.48% of the variance in the target variable. This suggests that there is still room for improvement in model performance.

Next Steps that could be utilized, include: Feature Selection and Engineering: Review features and consider adding new features or transforming existing ones. Try Different Models: Experiment with different regression algorithms like Random Forest, XGBoost, or even neural networks if appropriate. More Data: If possible, consider obtaining more data to train your model, as more data can often lead to better performance. Ensemble Techniques: Combine the predictions of several models to improve overall performance.
 
*Results:*

	•	User inputs the drug in question into a Gradio interface.
	•	The model checks for the correct information from the requested drug and summerizes the information.
 	•	The output is shown through the Gradio interface of the drug data including the side-effects.

*Gradio:*

	![Gradio Display](images/Gradio - Drug Interface Project 3.jpg)
 
*Contributors:*

	•	Kavita Gopal
	•	Tuan Huynh
	•	Jaiden Flint

*Future Work:*

	•	Expand dataset for broader drug variety.
	•	Optimize model for mobile devices.
	•	Explore model interpretability for safer usage in healthcare.
 	•	Using more powerful GPUs to process more data to improve accuracy.
	•	Provide images or video to help the user understand the drug in more detail.

 *References:*

 	•	https://www.kaggle.com/datasets/ahmedshahriarsakib/assorted-medicine-dataset-of-bangladesh?select=generic.csv
 	•	https://colab.research.google.com/
  	•	https://gemini.google.com/
 	


