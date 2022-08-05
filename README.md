# Module_11 - Time Series

   ![Charts Picture](Images/11-4-challenge-image.png)

With over 200 million users, MercadoLibre is the most popular e-commerce site in Latin America.  As one of their growth analysts, I've been tasked with analyzing the company's financial and user data in clever ways to make the company grow.  Here, I'll be finding out if the ability to predict search traffic can translate into the ability to successfully trade the stock.

---

## Technologies

This Jupyter Notebook was uploaded and run in Google Colab to help with issues with FB Prophet running on my machine via Jupyter Labs.  To access the notebook directly from my Google Colab Drive, navigate to https://colab.research.google.com/drive/1TLFneEL1z_A8PuZFJL9osUKnEK5Cv7LN?usp=sharing 

It leverages python 3.7.11 with the following packages:

* [pandas](https://pandas.pydata.org) - Use the Pandas library, along with JupyterLab, to collect, prepare and analyze data.

* [FB Prophet](https://github.com/facebook/prophet) - Automated time series forecasting procedure.

* [pystan](https://pystan.readthedocs.io/en/latest/) - Python interface to Stan, a package for Bayesian inference.

* [HoloViz (formerly PyViz)](https://holoviz.org) - Data visualization tool hvPlot.

* [numpy](https://numpy.org/doc/stable/) - Fundamental package for scientific computing in Python.

---

## Installation Guide

First install the required libraries:

```python
  !pip install pystan~=2.14
  !pip install fbprophet
  !pip install hvplot
  !pip install holoviews
```

Before running the application first import the following libraries and dependencies:

```python
  import pandas as pd
  import holoviews as hv
  from fbprophet import Prophet
  import hvplot.pandas
  import datetime as dt
  import numpy as np
  %matplotlib inline
```

---

## Usage

The notebook has 5 main subsections, each of which contain the instructions, code, plots and answers to any specific questions for each of the 5 steps of this project:
* Step 1: Find unusual patterns in hourly Google search traffic
* Step 2: Mine the search traffic data for seasonality
* Step 3: Relate the search traffic to stock price patterns
* Step 4: Create a time series model with Prophet
* Step 5 (optional): Forecast revenue by using time series models

---

## Contributors

Starter code was provided by UW Fintech Bootcamp.  Updates and analysis by Jason Buckholt.  

---

## License

MIT License

Copyright (c) 2022 Jason Buckholt

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.