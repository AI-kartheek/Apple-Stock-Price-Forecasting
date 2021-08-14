
# Apple Stock Price Forecasting

## Overview
**`Stacked LSTM`** in Keras API is used to train Apple Stock (**`Close`**) Data to analyse and forecast the future stocks in Apple company.
* Model trained on Apple Stock Data that had been collected from [Tiingo](https://www.tiingo.com/) from Date **2016-07-28** till **2021-07-26** (or) [download](https://raw.githubusercontent.com/AI-kartheek/Apple-Stock-Price-Forecasting/main/datasets/Apple%20Stock%20Price.csv) the same dataset used in this project.
* Trained Model (`saved models`/`Stacked LSTM for Apple Stocks.h5`) takes previous 100 days stock (Close) data as input and can forecast on (Close) stock on specified N number of days.
* Model `trained` on ***717*** records and `tested` on ***340*** records.
* Model trained on 15 epochs with early stopping and model check point on decreasing validation loss, there by **Trian_loss**: `8.7085e-04` - **Val_loss**: `0.0366`.

![](https://raw.githubusercontent.com/AI-kartheek/Apple-Stock-Price-Forecasting/main/Images/Model%20performance.jpg)

## Installation
The Code is written in Python 3.8.5. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip.

* to create a [virtual environment](https://www.javatpoint.com/how-to-create-a-virtual-environment-in-python) if you wish.

Activate virtual environment if created and to install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
```bash
pip install -r requirements.txt
```
> All the Code Explanation of this Project had been explained [here](https://github.com/AI-kartheek/Apple-Stock-Price-Forecasting/blob/main/stacked%20LSTM%20for%20Apple%20stock%20market%20prediction%20and%20forecasting.ipynb) right from ``Data Collection`` till ``Forecasting``.

## Notebook Summary
* Collect Stock Data
* Load Data
* Train Test Split
* Data Sequencing
* MinMax Scaling
* Reshape into 3D data
* Model Creation
* Load Saved Model
* Analyse RMSE
* Plotting Results
* Forecast on future 30 days
