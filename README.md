# Snetiment_Model_Template
The ultimate template to build a Sentiment Model starting from Linear SVM to Word2Vec 

 This repo is in ``` Python 2 ```

 - This repo consists of the following files:
 	1. Sentiment_Models_Template.ipynb --
 			Which contains the sentiment model meat
 	2. utils.py --
 			A python script that conatins some function to plot the learning curve, confussion matrix, and validation curve to assest the model
 	3. logistic_reg_inspection.py --
 			A python script that contains code to check what the model learnt using logistic regression coeffecients
 			To use it, you need to do the following:
			
```python
importance = get_most_important_features(vectorizer, log_clf, 10) # log_clf is the LogisitcRegressin Model
top_scores = [a[0] for a in importance[0]['tops']]
top_words = [a[1] for a in importance[0]['tops']]
bottom_scores = [a[0] for a in importance[0]['bottom']]
bottom_words = [a[1] for a in importance[0]['bottom']]

plot_important_words(top_scores, top_words, bottom_scores, bottom_words, "Most important words for Sentiment")
```

 	4. data --
 	   Is the folder that will contain your data
	   
	5. cleaned_data --
	   Contains the data after cleaning

