# Natural-Language-Processing-Crowdsourced-recommendation
Build a crowdsourced recommendation system from user reviews of beers from beeradvocate.com

## Objective: 
The objective is to create the building blocks of a crowdsourced recommendation system. This recommendation system will accept user inputs about desired attributes of a product and come up with recommendations. For this, we will scrape reviews of craft beer from beeradvocate.com.  
Assume that a customer, who will be using this recommendation system, has specified 3 attributes in a beer. Consider the below list for beer attributes.

  •	Aggressive (Boldly assertive aroma and/or taste)
  
  •	Balanced: Malt and hops in similar proportions; equal representation of malt sweetness and hop bitterness in the flavor — especially at     the finish
  
  •	Complex: Multidimensional; many flavors and sensations on the palate
  
  •	Crisp: Highly carbonated; effervescent
  
  •	Fruity: Flavors reminiscent of various fruits or Hoppy: Herbal, earthy, spicy, or citric aromas and flavors of hops or Malty: Grainy,       caramel-like; can be sweet or dry
  
  •	Robust: Rich and full-bodied

## Approach
1. Choose three attributes from the above list. We will perform a word frequency analysis of the data to make sure that the three given attributes are actually mentioned.   
2. Perform a similarity analysis using spacy with the 3-attribute set and the reviews. From the output file, choose 300 reviews that have the highest similarity scores with the attribute set you have chosen. 
3. Perform sentiment analysis using VADER on these 300 reviews and sort them (high to low) by the sentiment scores.
4. Based on the above analysis, recommend 3 beers to the customer. 

### Recommendation result comparison:
How would the recommendations differ if we ignore the similarity and sentiment scores and simply chose the 3 highest rated beers from the entire dataset? 

