# SuperStore
The explosive growth of online content and services has provided a myriad of choices for users. Therefore, personalized recommendations are necessary to improve user experience and ensure retention. 
The corollary of pleasant and convenient user experience is augmented profits for businesses. Before curating a set of products for different users, it is imperative to understand them better. Every customer is unique. Hence, if you treat them the same way with the same content, same channel, same importance, they will find another option which understands them better.
We segment the users based on RFM Modelling and create personalised Recommender System models based on Collaborative filtering. 
In order to tackle the cold-start problem i.e. when new user opens the app we recommend popular items
Users can search for products and with product similarity search we display similar products to product that user searched for

# Project Proposal
CLAAT: https://codelabs-preview.appspot.com/?file_id=1v93fwAPwqChS22TUFjwjyT-RNtvWgNpaRr53NvFMF3U#0

# Report
CLAAT: https://codelabs-preview.appspot.com/?file_id=1Sw4fG-F6BLDCx5oMwuYoyhWEHMqgGy9IXSjnGi7SklY#0

# Application URL
Heroku:

# Dashboard
https://datastudio.google.com/reporting/8fe1e49e-78be-4b1b-b2b5-94ad5d9db854
https://datastudio.google.com/u/0/reporting/8fe1e49e-78be-4b1b-b2b5-94ad5d9db854/page/UIhtB

# Approach
1. We performed EDA and analyzed customer behavior trends to better understand our customer's data 
2. We segmented the customers using RFM Modelling based on their purchasing history. Also, calculated the CLV to understand the importance of each customer.
3. We provided personalised recommendations to users by predicting their ratings based on collaborative filtering
4. We excecuted 4 collaborative models and compared its evaluation metrics to chose the model most ideal model for our prediction
5. For new users we recommend products based on popularity
6. The users have an option to search for products and get a list of products similar to their search
7. We created an interactive dashboard to analyze the sales based on customer segments.

# Customer Segmentation
• We cannot treat every customer with the same importance.They will find another option which understands them better.
• Each customer has a different profile and we need to tailor our recommendations based on their profiles. 
• In order to better understand our customers we segment our customers based on their RFM values.
• By using the RFM score we segment our customers into Top,Lost and Regular customers

# Recommendation
 • A recommender system predicts the rating value of a user-item combination with an assumption that the training data available indicates a user’s preference for other items.
 • We use the user-item Interaction Data, such as ratings and apply various modelling techniques that uses collaborative filtering to predict user’s preference.
 • We executed 4 collaborative modelling techniques :
            •FASTAI    •Alternating Least Square (ALS)  •Simple Algorithm for Recommendation (SAR)  •Surprise Singular Value Decomposition (SVD)
 • We compared the evaluation metrics and chose SVD as most ideal for our dataset 
 • Based on the predicted ratings we recommended top-k items to a particular user.
 • For new users as we do not have their pereferences we recommend most popular products.
 • We check for products which are most purchased and are highly rated to recommend those for new users


# Search 
 • Users can find the products they are looking for using the Search feature
 • The search feature also lists the products similar to the items being searched
 • We used text processing to find similar products.
 • We created a Document Term Matrix using TF-IDF to extract vectors
 • Using cosine similarity we calculated proximity between strings
 • Based on similarity values we created product groups
  

# Application Navigation
### 1. Welcome Page
Superstore home page

### 2. Login 
When a user login using their credentials, personalised recommendations are provided 

### 3. Search
When a customer searches a product,the app displays the product searched and also the similar products to the search

### 4. New Customer
When a new customer opens the app,product recommendations are provided based on popularity



