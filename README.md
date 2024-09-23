# Twitter Mood predicts the Stock market

This is my project during my Research Internship where I have studied about the effects of twitter tweets on the stock index or the stock price of a particular company (NetFlix).
The aim was to increase the accuracy of prediction of the stock index by also including another variable- Tweet factor, which represesnts
the public sentiment about that company a few days prior, which further aids in predicting the stock index in the near future.


## Background:

### Why Use LSTM for Time Series?

Time series data is inherently sequential, with each data point dependent on previous ones. Traditional models like ARIMA and even basic neural networks often struggle to capture complex temporal relationships, especially over long sequences. LSTMs offer several advantages:

**Memory Capability:** Ability to remember information over long sequences.

**Handling Non-Linear Relationships:** Can model complex, non-linear patterns in data.

**Flexibility:** Applicable to a wide range of time series tasks, including forecasting, classification, and anomaly detection.

**Adaptability:** Can be combined with other neural network architectures (e.g., CNN-LSTM) for enhanced performance.

### CNNs for Time Series:

While traditional time series models like ARIMA and state-of-the-art models like Recurrent Neural Networks (RNNs) have their strengths, CNNs offer unique advantages:

**Feature Extraction:** CNNs automatically learn hierarchical features from raw data without the need for manual feature engineering.

**Parallelism:** Unlike RNNs, CNNs can process entire sequences simultaneously, leading to faster training times.

**Local Pattern Recognition:** CNNs excel at detecting local dependencies and patterns, which are common in time series data.

**Flexibility:** They can be integrated with other neural network architectures to enhance performance.

### ARIMA:

**ARIMA**, which stands for **AutoRegressive Integrated Moving Average**, is a widely used statistical model for analyzing and forecasting time series data. It is particularly effective for datasets that exhibit patterns over time, such as trends or seasonality. ARIMA models are powerful because they combine three key components to capture different aspects of a time series:

**AutoRegressive (AR):**
This part of the model uses the relationship between an observation and a specified number of lagged observations (previous time points).
Parameter p: Denotes the number of lagged observations included in the model.

**Integrated :** This involves differencing the data to make the time series stationary, which means its statistical properties (like mean and variance) are constant over time.
Parameter d: Represents the number of times the data needs to be differenced to achieve.

**Moving Average (MA) :** This part models the relationship between an observation and a residual error from a moving average model applied to lagged observations.
Parameter q: Indicates the number of lagged forecast errors in the prediction equation.

## Project Structure:

1.Stock Data Scraping

2.Twitter Data Scraping

3.Twitter Data Preprocessing and Sentiment analysis ( https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment )

4.Modeling Using Two approaches

5.ARIMA as Baseline

6.Deep learning architecture using 1D-CNN and BiCudaLSTM layers as our new approach

7.Compare and evaluate our approach vs ARIMA

8.Evaluate our approach against new data in real-time
