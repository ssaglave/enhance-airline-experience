**Title:** Enhanced Airline Customer Experience through Sentiment-Driven Topic Modeling and Actionable Insights. 
 
**Project Description:** Built a topic modeling system that can be used to provide recommendations to enhance customer satisfaction based on negative reviews from British Airlines Customer Reviews. This system will perform sentiment analysis on all airline reviews to determine positive and negative reviews from customers. Next, negative reviews are used to determine the nature of the issue and group them to related common issues and provide topics. These labels/topics would then be used to provide actionable recommendations to improve service quality. 
 
**Data sources:** Kaggle link (https://www.kaggle.com/datasets/chaudharyanshul/airline-reviews)
 
**Project Pipeline:**
 
**1.	Data Preprocessing:**  
•	Performed cleaning on the data by removing special characters, numbers, and stop words. 
•	Tokenizing and lemmatizing the reviews for better analysis. 
 
**2.	Sentiment Analysis:**
•	Classify reviews as positive or negative. 
•	Model#1 used BERT. 
•	Model#2 used RoBERTa.
•	Evaluation metrics: Accuracy, Precision, Recall, and F1 score. (using recommended column as gold labels for this task) 

**3.	Custom Data Labeling:**
•	Worked on 1100 negative reviews to add custom labels manually based on common issues identified.
•	Add custom topics using an open-source data labeling tool - Label Studio (https://labelstud.io/guide) by grouping negative reviews ex: Seat Comfort, Flights Delays and Cancellations, Food and beverage, etc.

**4.	Topic Modeling:**
•	Get topics for the negative reviews from this task.  
•	Model#1 used Latent Dirichlet Allocation (LDA). 
•	Model#2 used BERTopic. 
•	Evaluation metrics: coherence scores and topic diversity.  
 
**5.	Evaluation and Comparison:** 
Compare manual topics with BERT topics using: 
•	BERT score (precision, recall, f1 score) 
 
**6.	Future work:** 
Explore generating recommendations/improvement suggestions based on identified topics using GPT-4 or Olama.  
 
**Computational Resources:**  
We plan to use Hugging Face’s transformers (BERT, RoBERTa and BERTopic), open-source Label Studio for custom topic labeling.
