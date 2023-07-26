# Coding Challenge Huk-Coburg

The four notebooks have the following content:
*  exploration.ipynb - Data Exploration and Preperation
*  modelling_ClaimNormPrediction.ipynb - Experiment to predict a normalised Claim Amount directly from the features
*  modelling_AmountPrediction.ipynb - Experiment to predict Claim Amount trained only on positive cases
*  modelling_claimprediction.ipynb - Experiement to predict likelihood of a Claim

### Final Statement

It proved to be difficult to predict the amount of individual claims as well as the combination of amount and claim/no-claim (R2 around 0). Propbably to the high randomness of both, the occurance of a claim and the amount of the claim.

The proposed way to model the claims is to take the predicted probabilities from the best ML model as a factor for individual claim likelihood. By scaling to average number of claims and average amount per claim, a claim-amount model can be created.


### Future Work

* Futher hyperparameter tuning and additional models
* Include exposure as factor into the model
* Multiple claims for an individual have been ignored (duplicate datapoint?)
* In-depth feature analysis

