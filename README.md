While looking for anomaly detection techniques one will come across wealthy sets of techniques online, which range from statistical methods to machine learning to neural network (of course. NN can do anything lol). One particular detection method caught my eyes recently and it reads:

> _"The underlying algorithm – referred to as Seasonal Hybrid ESD (S-H-ESD) builds upon the Generalized ESD test for detecting anomalies. Note that S-H-ESD can be used to detect both global as well as local anomalies. This is achieved by employing time series decomposition and using robust statistical metrics, viz., median together with ESD. In addition, for long time series (say, 6 months of minutely data), the algorithm employs piecewise approximation - this is rooted to the fact that trend extraction in the presence of anomalies in non-trivial - for anomaly detection."_

That's right! That's Twitter Anomaly Detection from Twitter (it's only in R now. Twitter data scientists uses R mainly?) and it was introduced mainly for time series data.

**But I've have never heard of ESD**. What makes me excited about learning more is that

1. it's built upon some easy-to-understand statistical calculations and transparent process.
2. Student's t-distribution is used. The familiar hypothesis testing concept is used.
3. I feel it's simpler to understand than Prophet's Fourier Transform and some Bayesian.

To understand Twitter's Anomaly Detection underlying algorithm, we need to start from the basics. ESD stands for Extreme Studentized Deviate. Generalized ESD is an extension of Grubb's test. The notebook in this directory aims to explain Grubb's test, G-ESD and Twitter's Anomaly Detection with example codes and then demonstrate Twitter's package with 2 very different kind of datasets.
