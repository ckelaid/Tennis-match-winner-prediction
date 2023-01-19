# Tennis-match-winner-prediction

In this project, I built a scraper to scrape tennis match statistics from atptour.com, and then a tool that uses the statistics to predict the winner of a tennis match and in doing so identifies which variable was of most importance in the prediction of the winner.



### EDA

Some basic EDA to see how varibales relate to eachother

<p float="left">
  <img src="Images/retpts_vs_totpts.png" width="500" height="300" />
  <img src="Images/servepts_vs_1stserve.png" width="500" height="300" /> 
</p>

<img src="Images/totpts_vs_servepts.png" width="500" height="300"> 


### Variable Selection

Here I performed **Best Subset Selection** and use BIC, Adj-R2 and Cp to evaluate the models based on the number of variables

<img src="Images/BSS_scores.png" width="700" height="300" />

Also performed Lasso using CV to pick the best $\lambda$ value and see what how many and which variables were picked in this case

<img src="Images/Lasso_lambda.png" width="600" height="300" />

Ended up being between a 4 to 7 variable model.


### Model Fitting & Evaluation
