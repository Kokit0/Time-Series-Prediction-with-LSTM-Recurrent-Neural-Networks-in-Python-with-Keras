# Time Series Prediction with LSTM Recurrent Neural Networks in Python with Keras


by **[Jorge Amaya S.](https://www.linkedin.com/in/jorge-amaya-soto)** on July 27, 2023 inspired in **[Deep Learning for Time Series](https://machinelearningmastery.com/category/deep-learning-time-series/)**

**Last Updated on August 7, 2022**

Time series prediction problems are a difficult type of predictive modeling problem.

Unlike regression predictive modeling, time series also adds the complexity of a sequence dependence among the input variables.

A powerful type of neural network designed to handle sequence dependence is called a [recurrent neural network](https://machinelearningmastery.com/crash-course-recurrent-neural-networks-deep-learning/). The Long Short-Term Memory network or LSTM network is a type of recurrent neural network used in deep learning because very large architectures can be successfully trained.

In this post, you will discover how to develop LSTM networks in Python using the Keras deep learning library to address a demonstration time-series prediction problem.

After completing this tutorial, you will know how to implement and develop LSTM networks for your own time series prediction problems and other more general sequence problems. You will know:

- About the International Airline Passengers time-series prediction problem
- How to develop LSTM networks for regression, window, and time-step-based framing of time series prediction problems
- How to develop and make predictions using LSTM networks that maintain state (memory) across very long sequences

In this tutorial, we will develop a number of LSTMs for a standard time series prediction problem. The problem and the chosen configuration for the LSTM networks are for demonstration purposes only; they are not optimized.

These examples will show exactly how you can develop your own differently structured LSTM networks for time series predictive modeling problems.

**Kick-start your project** with my new book [Deep Learning for Time Series Forecasting](https://machinelearningmastery.com/deep-learning-for-time-series-forecasting/), including *step-by-step tutorials* and the *Python source code* files for all examples.

Let’s get started.

- **Jul/2016**: First published
- **Updated Jul/2022**: Updated for TensorFlow 2.x

### **Updated LSTM Time Series Forecasting Posts:**

The example in this post is quite dated. Jason Brownlee made some newer versions of this topic. check them out too! You can view some better examples using LSTMs on time series with:

1. [LSTMs for Univariate Time Series Forecasting](https://machinelearningmastery.com/time-series-forecasting-long-short-term-memory-network-python/)
2. [LSTMs for Multivariate Time Series Forecasting](https://machinelearningmastery.com/multivariate-time-series-forecasting-lstms-keras/)
3. [LSTMs for Multi-Step Time Series Forecasting](https://machinelearningmastery.com/multi-step-time-series-forecasting-long-short-term-memory-networks-python/)

![Photo by [ X Y Z ](https://www.flickr.com/), some rights reserved.]

Photo by [Margaux-Marguerite Duquesnoy](https://www.flickr.com/photos/124559226@N08/15792381395/), some rights reserved.

Time series prediction with LSTM recurrent neural networks in Python with Keras