# Recommender_Systems
Traditionally, recommender systems are based on methods such as clustering, nearest neighbor and matrix factorization. However, in recent years, deep learning has yielded tremendous success across multiple domains, from image recognition to natural language processing. Recommender systems have also benefited from deep learning's success. In fact, today's state-of-the-art recommender systems such as those at YouTube and Amazon are powered by complex deep learning systems, and less so on traditional methods.
In this notebook, we’ll go through the following:
How to create your own deep learning based recommender system using PyTorch Lightning
The difference between implicit and explicit feedback for recommender systems
How to train-test split a dataset for training recommender systems without introducing biases and data leakages
Metrics for evaluating recommender systems (hint: accuracy or RMSE is not appropriate!)
#Datasets
https://www.kaggle.com/grouplens/movielens-20m-dataset
#Building Recommender Systems using Implicit Feedback
Explicit Feedback
In the context of recommender systems, explicit feedback are direct and quantitative data collected from users. For example, Amazon allows users to rate purchased items on a scale of 1-10. These ratings are provided directly from users, and the scale allows Amazon to quantify user preference. Another example of explicit feedback includes the thumbs up button on YouTube, which captures users' explicit preference (i.e. like or dislike) of a particular video.
However, the problem with explicit feedback is that they are rare. If you think about it, when was the last time you clicked the like button on a YouTube video, or rated your online purchases? Chances are, the amount of videos you watch on YouTube is far greater than the amount of videos that you have explicitly rated.
Implicit Feedback
On the other hand, implicit feedback are collected indirectly from user interactions, and they act as a proxy for user preference. For example. videos that you watch on YouTube are used as implicit feedback to tailor recommendations for you, even if you don't rate the videos explicitly. Another example of implicit feedback includes the items that you have browsed on Amazon, which are used to suggest other similar items for you.

The advantage of implicit feedback is that it is abundant. Recommender systems built using implicit feedback also allows us to tailor recommendations in real time, with every click and interaction. Today, online recommender systems are built using implicit feedback, which allows the system to tune its recommendation in real-time, with every user interaction.
#Result
We got a pretty good Hit Ratio @ 10 score! To put this into context, what this means is that 86% of the users were recommended the actual item (among a list of 10 items) that they eventually interacted with. Not bad!

