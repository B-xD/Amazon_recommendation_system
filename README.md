# Amazon_recommendation_system
In this project we will work with the Amazon product reviews dataset to create various recommendations systems and pick the best one 

## Objective
Develop a recommendation system that suggests products to customers based on their previous ratings of other products. You will utilize a dataset containing labeled Amazon product reviews to extract insights and build an effective recommendation system.

## Dataset
The Amazon dataset includes the following attributes:
- **userId**: Unique identifier for each user.
- **productId**: Unique identifier for each product.
- **Rating**: Rating given by the user to the corresponding product.
- **timestamp**: Time of the rating (not used in the current analysis).

### Note
The project includes user-defined functions for making recommendations and measuring model performance. You may use these functions or create your own as needed.

**Installation Note**: To avoid issues with the installation of the `surprise` library (used for building recommendation systems), it is recommended to use **Google Colab** for this project.

## Models Analyzed
In this study, we built and evaluated several models for the recommendation system, including:
1. **Rank-Based Recommendation System**
2. **User-User Similarity-Based Recommendation System** using KNNBasic
3. **Item-Item Similarity-Based Recommendation System** using KNNBasic
4. **Matrix Factorization-Based Recommendation** (SVD)

## Conclusion and Recommendations
All models indicated that the recommended items were relevant to the selected users (ratings above the 3.5 threshold). Despite their differences, the models performed similarly.

Based on the metric of interest, the **F1-score**, the best-performing model was the **User-User Similarity-Based Recommendation System**, achieving an F1-score of **83.1%** and predicting a score of **4.29** for user ID "A3LDPF5FMB782Z," which closely aligned with the actual score of **5**. The SVD model followed as the second-best option.

### Recommendations
To enhance the relevance of recommendations and increase purchase likelihood:
- **Deploy the User-User Similarity-Based Recommendation System** as the primary model on the Amazon platform.
- Encourage user interaction by prompting customers to rate products, leave reviews, and provide feedback. Increased user engagement will help validate model performance and gather more data for improvement.
- Continuously assess the model's performance to ensure it remains effective over time.

By implementing these recommendations, Amazon can improve its recommendation capabilities, leading to higher customer satisfaction and increased revenue.
