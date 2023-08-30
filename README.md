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

## SETUP INSTRUCTIONS:

```markdown
This repository contains code for time series prediction using an LSTM neural network. The code requires the following libraries: pandas, numpy, matplotlib, scikit-learn, tensorflow, Seaborn, and keras.

## Setup Instructions

Follow these steps to set up your environment and run the code:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/Kokit0/Time-Series-Prediction-with-LSTM-Recurrent-Neural-Networks-in-Python-with-Keras
   ```

2. Navigate to the project directory (Change the name if you like):

   ```bash
   cd your-repo
   ```

3. Create a virtual environment and activate it:

   On Windows:

   ```bash
   python -m venv venv_minimal
   .\venv_minimal\Scripts\Activate
   ```

   On macOS and Linux:

   ```bash
   python3 -m venv venv_minimal
   source venv_minimal/bin/activate
   ```

4. Install the required packages:

   ```bash
   python.exe -m pip install --upgrade pip
   
   pip install -r requirements.txt
   ```

5. Run the code:

   You can run the code in your Jupyter Notebook, VSCode or Python environment.

6. Deactivate the virtual environment:

   ```bash
   deactivate
   ```

## Troubleshooting

If you encounter any issues during the setup process, feel free to reach out for help. Happy coding!
```
