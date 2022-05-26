# Modeling Grocery Prices In Seven Countries Using Bayesian Statistics

### Motivation

This project was created for my CS146 class: Computational Methods for Bayesian Statistics. 

Using student-collected data from 7 countries (USA, Canada, Bangladesh, Brazil, Kenya, Sweden, Ukraine) during March 2020, I create a model to help answer questions like:

- How (or do) do grocery prices vary by country and store brand level (budget, mid-range, luxury)?
- Are grocery prices and the geographical distribution correlated with other cost-of-living measures?


These questions are attempted to be addressed by utilizing Bayesian Statistics and PyStan functionality available in Python. Model setup and conclusions are described below.

### Dataset
- Data was collected during from February 28 2020 to March 10 2020
- Data was collected from the following countries: USA, Canada, Bangladesh, Brazil, Kenya, Sweden, Ukraine, with varying quantities of observations from each country
- The price of the following products were collected: apples, bananas, tomatoes, potatoes, flour, rice, milk, butter, eggs, chicken breasts
- Additionally, the average cost of a rental nearby was collected as the reference for cost-of-living

### Modeling
The basic idea of the model is that each type of product has a base price, with multipliers depending on store brand and geographical location which can influence the final price

### Results
For additional results, see the ipynb notebook.
The posterior probability of the results were calculated and are visible below.

<img width="844" alt="image" src="https://user-images.githubusercontent.com/55218727/170592586-0a60ad86-5dd5-48a1-bfbf-5a12614b305e.png">
<img width="482" alt="image" src="https://user-images.githubusercontent.com/55218727/170592616-a6826b62-0688-45b4-a7a7-240d7062117b.png">

Ultimately, it was shown that the country where the item was purchased had a greater effect on the price than the store type.
