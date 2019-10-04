# Time series forecasting

This is the repository for the practices of "Time series analysis", a graduate course at FaMAF's #DiploDatos, National University of Córdoba

Based in "A short course on forecasting" by Marcel Scharth, The University of Sydney.

This material draws on the [Forecasting Principles and Practice](https://www.otexts.org/fpp2) textbook by Rob Hyndman and George Athanasopoulos. While the textbook and Rob Hyndman's [DataCamp course](https://www.datacamp.com/courses/forecasting-using-r) use R, our tutorials provide a Python version of related content, but based only in [**statsmodels**](https://www.statsmodels.org) and the [scipy stack](https://www.scipy.org/stackspec.html).

This version: September 6, 2019.

## Tutorials (Python)

* [Working with time stamped data in Python](https://github.com/gmiretti/forecasting/blob/master/Tutorial01%20Time%20Stamped.ipynb)
* [Introduction to forecasting](https://github.com/gmiretti/Forecasting/blob/master/Tutorial02%20Forecasting.ipynb)
* [Holt-Winters smoothing](https://github.com/gmiretti/Forecasting/blob/master/Tutorial03%20Holt%20Winters%20Smoothing.ipynb)
* [ARIMA](https://github.com/gmiretti/Forecasting/blob/master/Tutorial04%20ARIMA.ipynb)
* [Seasonal ARIMA](https://github.com/gmiretti/Forecasting/blob/master/Tutorial05%20Seasonal%20ARIMA.ipynb)

## Execution

### Conda

Install requirements using command bellow and then open Jupyter notebook:

    conda install --file conda-requirements.txt

### Docker

Run and then go to http://localhost:8889

    docker run -p 8889:8888 gmiretti/forecasting

To update to latest version execute the command below and run again:

    docker pull gmiretti/forecasting

