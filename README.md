### Motivation:

[ProductHunt.com](https://www.producthunt.com) is a collection of product postings on which visitors can comment and upvote. Companies (or small teams, or even individuals) can post their products on ProductHunt in an effort to disseminate it to ProductHunt’s large audience.
[Data.world](https://data.world) has compiled the most comprehensive ProductHunt dataset ever released. 2 years of posts, votes, taglines, and more!

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/10040565/23584466/25dfb448-0128-11e7-9d8e-02e0abef4636.png" width="400"/>
</p>

Recently, **data.world** and **Galvanize** organized a **mini-hackathon** in an effort to discover which types of products tend to perform well, and possibly discover why. My team won the **“Best Visualization”** category for producing a “story” of
sequential visualizations exploring the differences between highly up voted posts and posts that don’t generate a lot of interest on product hunt.
In addition to the analysis done at mini-hackathon, I have also added a prediction model to predict the number of votes a product can get.

### Data:
There are 3 datasets available.
1. Topics: Description of each topic to which the product can belong to.
2. Product posts: Description of each product posted.
3. Users: Details of users.
The extract is from 24-Nov-2014 to 21-Nov-2016.
The extract is available [here](https://data.world/producthunt/product-hunt-research)


### Project Scope:
1. Which topics are more successful?
2. Model to predict if a product will be successful.


### Explore data:
1.**Product creation trends:**
The trend shows that very few products are created during the evening and afternoon. Products are mostly
created during the night and morning. In 2016, products were mostly created at night.

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/10040565/23671870/6dfbb388-0332-11e7-97c6-4b2674fbbdee.png" width="800"/>
</p>

2.**User activity:**
Users active on social media(have a twitter account) also tend to be active on ProductHunt.

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/10040565/23676863/a7ad1750-0343-11e7-94e1-99fa1e38b86f.png" width="270"/>
</p>

Users with an updated profile also are more active on ProductHunt.

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/10040565/23676867/aa17feba-0343-11e7-8e16-d7cb56eb5ee1.png" width="270"/>
</p>




**Which topics are most successful?**
A topic is a group of similar products. A topic is considered successful if products in that topic has a high number of votes compared to products in other topics. Below is the list of the most successful topics based on its product votes.

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/10040565/23585364/8bfea530-0142-11e7-849b-ebb558244879.png" width="800"/>
</p>

**Model to predict if a product is successful**
The goal here is to use the features available when a product is posted and build a model to predict if that product will be successful. A product is defined as successful if the number of votes it receives is above the 75 percentile. The technical details of the model is here. 
I used Support vector Machine algorithm to classify a product as successful or not. The model has an accuracy of 98.6% and a recall of 94.6%
