# Chatbot_QA_Data_Augmentation_and_Evaluation

### How to Evaluate and Improve Performance of a LLM Chatbot by augmenting Data using LLM itself

It’s common nowadays for companies to use chatbots to process customers’ questions and requests. Most of us know that we can use the RAG (Retrieval Augmentation Generation) technique and Langchain to build such a chatbot.

However, when I was learning to build the chatbot application, several questions came to my mind: 
-	How do I know if my chatbot is answering the question correctly before I push it to production? 
-	Do I need to find another human to come up with testing questions and then review the answers manually? This seems to be a very unrealistic and inefficient approach.

Luckily, Langchain has developed and provided us another useful tool for efficiently generate and evaluate our LLM applications.

In this notebook, you will find codes which demonstrate:
1)	How to use LLM itself to help us generate new Question-Answer pair based on provided data context
2)	How to evaluate our LLM Chatbot answer performance on those newly generated questions
3)	How to improve our LLM Chatbot based on the evaluation

When I tested this myself using the code and dataset in the notebook, the chatbot’s performance (ability to answer the customers’ questions correctly) was improved from 79% to 93%. It originally would get confused by questions with different wordings and say it did not know the answer to many questions. After one round of data augmentation, the chatbot is able to score 14% more of correct answers [with extra new questions as test set]. It is quite an impressive performance gain. 

