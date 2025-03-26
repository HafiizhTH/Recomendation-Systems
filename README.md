# What is Recomendation Systems?

![Image](https://github.com/user-attachments/assets/87d6ff48-3619-4382-9ab8-1e48731b3fc8)

Recommendation system is a system that refers to predicting a number of items or data for users in the future, then making recommendations for the top items. One of the reasons why it is necessary to use a recommendation system is because users have many options to use due to the prevalence of the internet.

Although the amount of information available is increasing, a new problem arises as users struggle to select the items they want to view.

# Importance of Recommendation Systems

Recommender systems are an essential component of current digital platforms, helping to improve user experiences, drive engagement, and provide decision-making tools. These systems serve as information filtering tools, providing users with tailored material or information that is relevant to their taste and interests. Recommender systems have become essential for organizations since they can significantly boost income by making tailored suggestions that result in improved sales. 

- **Faster Decision-making**: Recommender systems increase user tendency to purchase suggested things, boost loyalty and overall happiness, lower transaction costs, and improve decision-making process and quality.
- **Personalized user experience**: Making highly relevant and valuable suggestions, recommender systems improve the user experience.
- **Increase engagement**: Recommendation systems help users interact with a system by providing them material, goods, or services that they are likely to be interested in.

# Recommendation System Method

![Image](https://github.com/user-attachments/assets/8d1b52ec-524a-4464-bfda-6cd9034bf66d)

The Recommendation System is divided into 3 methods:

- Content Based Recommendation
- Collaborative Filtering
- Content — Collaborative Recommendation (Hybrid Recommendation)


## Content Based Recommendation

Content Based Recommendation utilizes the information of several items/data to recommend to the user as a reference related to the information used previously. The purpose of content based recommendation is to be able to predict similarities from a number of information obtained from users.

For example, a user is watching a video on Youtube. The content viewed by the user is about soccer. Youtube will systematically recommend the user to view other videos related to soccer content.

In its creation, content based filtering uses the concept of vector calculation, TF-IDF, and Cosine Similarity which is essentially converted from data / text into a vector form.


![Image](https://github.com/user-attachments/assets/a326afe7-f14a-4221-b6a6-9ccaf5d363b8)


## Collaborative Filtering

Collaborative Filtering utilizes transactions of a product/item based on the user's behavior/habits. The goal is that the same user and similar items can be favored by users as recommendations for choice. 

Collaborative Filtering is generally divided into 2 methods:

- User-Based Collaborative Filtering (UB-CF)
- Item-Based Collaborative Filtering (IB-CF)

**User-Based Collaborative Filtering (UB-CF)** recommends product items by finding users who are similar to other users. For example, we want to recommend a movie to our friend. We can assume that similar people will have similar tastes. Suppose me and B have watched the same movies, and we rated them almost identical. But B hasn't seen the movie 'Harry Potter: Part II' and I have. If I like that movie, it's reasonable to think that he does too.

UB-CF has 2 calculation methods, namely Cosine similarity and Pearson Correlation.

Both methods are commonly used. The difference is that Pearson Correlation does not change to add a constant to all elements. In its construction, the commonly used algorithm is K-Nearest Neighbor (KNN). And the KNN algorithm can be seen in Scikit-learn.

**Item-Based Collaborative Filtering (IB-CF)** recommends similarities between items that target/interact with the user and other items. For example, a user likes the soccer team “Bayern Munich”. The system will automatically recommend items related to “Bayern Munich”, such as jerseys, balls, posters, and so on that are related.

In its creation, IB-CF uses the same calculation method as UB-CF. However, it is different in targeting a recommendation that is made.

In addition to the use of the KNN algorithm, collaborative filtering can also use the Matrix Factorization (MF) algorithm by decomposing the item-user matrix interaction into the product of two lower two-dimensional matrices. One matrix can be seen as the user matrix where rows represent users and columns are latent factors. The other matrix is the item matrix where rows represent latent factors and columns represent items.


## Content — Collaborative Recommendation (Hybrid Recommendation)

Hybrid systems in recommendation systems combine collaborative and content-based methods to leverage the strengths of each approach, resulting in more accurate and diversified recommendations. These systems often start with content-based filtering to study new users and gradually integrate collaborative filtering as more interaction data becomes available.

Hybrid recommender systems can be categorized into weighted, feature combination, cascade, feature augmentation, meta-level, switching, and mixed models. The feature combination method interprets collaborative information as additional feature associated with each example and applies content-based approaches to this enriched data collection. The meta-level hybrid recommender system combines two recommender systems such that the outputy of one becomes the input for the other.

Hybrid recommender systems are the most effective approach to developing a recommender system. However, they do have drawbacks, such as the ramp-up problem, since both systems need a database of ratings. Knowledge-based and utility-based recommender strategies . The most popular hybrid recommender systems are feature augmentation and meta-level systems, which feed information from one into the output of the other.

