# WLS-health-prediction
Predicting health outcomes from earlier survey data. 

In this project I search for correlations between parental socioeconomic status and health outcomes for their children. 

Data pulled from:
http://www.ssc.wisc.edu/wlsresearch/
http://www.ssc.wisc.edu/wlsresearch/documentation/waves/?wave=capigrad&module=jmail_health

In an earlier version of this project, I sought to use SF-12 scores as a proxy for general health and mental welfare outcomes and to predict SF-12 scores based on parental Socioeconomic Status, Family income, and gender. However upon ploting the mental and physical health scores against eachother, I found that the survey forces a trade off between physical and mental health scores, which leads to under estimating the mental stability of healthy people and under estimating the mental health of physically fit people. An example of this survey can be found and tested here for the same bias: http://www.sf-36.org/demos/SF-12.html

I believe the reason for the bias has something to do with Bayesian inference: if someone is in poor phyical condition but nevertheless has strong mental health, there is greater evidence that they are deeply mentally stable than someone who also has good health, but could become worse in terms of mental health if physical health were to decrease. Another posibility is that the designers of the scoring algorthim are activly trying to counter biases in responses: a person who ranks themselves as good in some things and bad at others is more likely to be telling the truth than someone who says they are good at everything or bad at everything. 

The inability to use such a score to quantify general health lead me to the approach of instead using many heath outcomes as "predictors" for parental SES in prior years. The outcomes that survived elastic net regularization are graphed and order by their regularized coefficients in this project. 

