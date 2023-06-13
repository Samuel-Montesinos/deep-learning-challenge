# Deep Learning Challenge

This repository is my attempt at understand Deep Learning and Neural Networks

## Purpose of the Analysis

The purpose of this analysis is to help us understand what factors affect the success of an organization funded by Alphabet Soup, and how likely they are to succeed

## Result

Although our model did not achieve the goal accuracy of 75%, we can still see a trend beginning to emerge. 

 - Data Preprocessing
* What variable(s) are the target(s) for your model?
* I focused on the IS_SUCCESSFUL column due to the fact that we should focus on all things that successful orgs have done that led to their success.
* What variable(s) are the features for your model?
* All other columns were features as these are showing us exactly what was done
* What variable(s) should be removed from the input data because they are neither targets nor features?
* The starter code helped with this, but the identification markers were omitted because they do not have an effect on the organization's success as they are serialized inputs.
 - Compiling, and training the model.
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
* I chose a variety of layers and activation functions to try and optimize the model. The initial code gave us a 71% success rate, so the next logical thing was to add more layers. Initially I tried four layers, with three being relu, and when this didn't work, I changed the avtivation to be sigmoid focused on three layers ro perhaps get a better output due to the non-binary nature of the data. I also tried using gridsearchCV and tried learning from documentation, but these results were fruitless as the data was far too large to be able to get the grid search done quickly and practically.
* Were you able to achieve the target model performance?
* As stated before, I was unable to reach the score of 75%. 

## Summary
In summary, our model will be able to identify a successful organization more often than not, however the results are not confident enough to justify its routine use. We could try a random forest model to further increase our accuracy. This model would work better as it allows the variables to be far more varied. Essentially the same justification that I had for using the sigmoid activation. The lack of binary data will impede the standard model. 

## Documentation used as reference
https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html
