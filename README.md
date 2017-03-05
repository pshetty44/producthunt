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
2. Prediction model to estimate upvotes for a product.


### Explore data:
A topic's success was defined by the total votes to the number of products in that topic.The below graph shows the top 50 popular topics.

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/10040565/23585304/c9a44824-0140-11e7-8da9-1ddaa35d19ec.jpg" width="400"/>
</p>
