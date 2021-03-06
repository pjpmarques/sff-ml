# Introdution

There are many books out there about Machine Learning (ML). Some quite deep and theoretical, some quite practical. In recent years there has also been a proliferation of frameworks and tools that you can use in a practical way to construct intelligent systems. Tools like [Scikit-Learn](http://scikit-learn.org/) is very well-known in the python community and useful for prototyping; [SparkML](http://spark.apache.org/docs/latest/mllib-guide.html) which runs to top of Spark and is able to process large volumes of information; or [TensorFlow](https://www.tensorflow.org/) that is gaining popularity for building "deep learning" models. These are just some examples, as there are tens of tools and libraries currently available. At the same time several companies are now trying to popularize the approach of "Machine Learning as a Service". Contenders include [Amazon's Machine Learning](https://aws.amazon.com/machine-learning/) and [Microsoft's Cortana](https://www.microsoft.com/en-us/cloud-platform/cortana-intelligence-suite). Stanford University even has its introductory [Machine Learning Course](https://www.coursera.org/learn/machine-learning) published on Coursera. It's an exciting time to be a Data Scientist!

### So, why a new book?

Although fraud is typically pointed out as one of the prime applications of Machine Learning, there is no book or guide out there that details on how to actually do it. At least, in a realist way. Developing a system for doing fraud prevention using machine learning is much more than creating a ML model. 

If you look at payments, over 99.95% transactions are not fraudulent. If you ask a computer to learn directly from the data, it will learn that nothing is fraud! And it will be right in 99.95% of the cases! Although correct, that's not very useful. So, you need to deal with things like "stratified sampling", "oversampling" and "undersampling". You also need to be able do design features from which your models can learn effectively -- what's called *feature engineering*.

In many cases you make create a model that detects fraud very well, but it takes to much time to do it. In the area of payments, it's common that you cannot take more than 1/10th of a second to decide if a transaction is good or not. Time is of essence because transactions occur in real-time. So, you need to be able to create models where timeliness is important. 

When you are evaluating results there are several metrics that are important. Fraud detection rate, false-positive rate, false-positive ratio, F1-measure, AOC, among others. In the case of fraud prevention some are more important than others. In this process, you need to be able to understand if you are really creating better models and if they are going to perform well when you move from the lab to production. Model evaluation and model calibration are very important.

Our objective with this book is to give an end-to-end guide to what it means to be a Data Scientist working on the area of Risk Management, in particular in Payments. A guide to the brave world of fighting fraud.

### Tools of the trade

For this journey we'll mostly use [Feedzai's Data Science Framework](https://www.feedzai.com). The main motivation is that same that lead to this book. Fighting fraud requires much more than simply creating an machine learning model. There are many tools and frameworks to create these models. But for doing the complete process that includes data exploration, sampling, feature engineering, profile building, model training and evaluation and production deployment, no tool currently rivals Feedzai's.
