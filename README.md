# WLS-health-prediction
Predicting health outcomes from earlier survey data. 

In this project I search for correlations between parental socioeconomic status and health outcomes for their children. 

Data pulled from:
http://www.ssc.wisc.edu/wlsresearch/
http://www.ssc.wisc.edu/wlsresearch/documentation/waves/?wave=capigrad&module=jmail_health

In an earlier version of this project, I sought to use SF-12 scores as a proxy for general health and mental welfare outcomes and to predict SF-12 scores based on parental Socioeconomic Status, Family income, and gender. However upon ploting the mental and physical health scores against eachother, I found that the survey forces a trade off between physical and mental health scores, which leads to under estimating the mental stability of healthy people and under estimating the mental health of physically fit people. An example of this survey can be found and tested here: http://www.sf-36.org/demos/SF-12.html

This lead me to the approach of instead using many heath outcomes as "predictors" for parental SES in prior years. The outcomes that survived elastic net regularization are graphed and order by their regularized coefficients in this project. 

