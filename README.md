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


*Results:*

	•	User inputs the drug in question into a Gradio interface.
	•	The model checks for the correct information from the requested drug and summerizes the information.
 	•	The output is shown through the Gradio interface of the drug data including the side-effects.


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
 	


