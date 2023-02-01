# Fintech-Project1- Group5


![Energy_usage_pic.jpg](https://github.com/vincentsgarzi/Group5Project1/blob/main/Images/Energy_usage_pic.jpg)

## Personal Energy Usage Analysis with capacity to predict future cost of energy. Tool utilizes analysis of a household's energy usage by regressing historical energy usage data and temperature. Local Temperature data is downloaded by an API connection with AERIS Weather. Tool can forecast what will happen to a household's energy usage when temperatures change per season going forward. Tool can also predict with a 95% certainty, what the household's future cost of energy will be. Tool calculates the correlation between average kWh price of energy in NY and both Natural Gas and Crude Oil prices. The tool then continues by automatically selecting the most correlated product to run a monte carlo simulation based on a seasonal selection of historical data to adjust for seasonal influence. Based on the predicted usage per season and the monte carlo simulations per season of the most correlated product the tool can predict the future cost of energy. 

## Personal_Energy_Usage_Final_2022_per_hr.ipynb
---

### This Jupyter notebook can be used as a template for to predict future cost of energy for a household, it utilizes SQL, Python and results can be displayed webbased via Viola library

The tool can help with analyzing future energy usage and predict the cost of energy going forward
* Anaylsis is done on the following steps: 
1. Analysis a households energy usage
2. Analysis of correlation between kWh prices and natural gas price and crude oil prices
3. Predict future kWh price based on most correlated product in above step adjusting for seasonal influence by running MC simuation based on season selection of historical data
4. Instructions on how to deploy the notebook as a web application


---
## Table of Content

- [Tech](#technologies)
- [Installation Guide](#installation-guide)
- [Usage](#usage)
- [Contributor(s)](#contributor(s))
- [License(s)](#license(s))

---
## Tech

This project leverages python 3.9 and Jupyter Lab with the following packages:

* `Python 3.9`
* `Jupyter lab`

* [JupyterLab](https://jupyter.org/) - Jupyter Lab is the latest web-based interactive development environment for notebooks, code, and data.

* [pandas](https://pandas.pydata.org/pandas-docs/stable/index.html) - Pandas is an open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language.

* [numpy](https://numpy.org/doc/stable/index.html) - NumPy is a package for scientific computing in Python.

* [dotenv](https://pypi.org/project/python-dotenv/) - Python-dotenv reads key-value pairs from a .env file and can set them as environment variables.

* [json](https://docs.python.org/3/library/json.html) -  JSON is a lightweight data interchange format inspired by JavaScript object literal syntax.

* [requests](https://requests.readthedocs.io/en/latest/) - Requests is an elegant and simple HTTP library for Python, built for human beings.

* [hvplot](https://hvplot.holoviz.org/user_guide/Plotting.html) - hvplot is generate plots from Pandas DataFrames and many other data structures of the PyData ecosystem.

* [sqlalchemy](https://www.sqlalchemy.org/) - SQLAlchemy is a Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL.

* [os](https://docs.python.org/3/library/os.html) - module provides a portable way of using operating system dependent functionality.

* [MCForecastTools](https://cdn.inst-fs-pdx-prod.inscloudgate.net/e0e08ad7-c5b3-43c1-8e7c-e7efc5f1f39c/MCForecastTools.py?token=eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCIsImtpZCI6ImNkbiJ9.eyJyZXNvdXJjZSI6Ii9lMGUwOGFkNy1jNWIzLTQzYzEtOGU3Yy1lN2VmYzVmMWYzOWMvTUNGb3JlY2FzdFRvb2xzLnB5IiwidGVuYW50IjoiY2FudmFzIiwidXNlcl9pZCI6IjE1MDQyMDAwMDAwMDA0MTkyOCIsImlhdCI6MTY3MjMwNDM5NywiZXhwIjoxNjcyMzkwNzk3fQ.WGJMX_rASeilWSbulLAihV6NgGxdQXfVJnemxa9Pdyydjy0LvqbqBUcMU_ORuels5eLcI8CUQ7bzjZMIcmOi3A&content_type=text%2Fx-python) -  A Python class for runnning Monte Carlo simulation on portfolio price data.

* [sklearn](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html) - LinearRegression fits a linear model with coefficients w = (w1, …, wp) to minimize the residual sum of squares between the observed targets in the dataset, and the targets predicted by the linear approximation.

* [voila](https://voila.readthedocs.io/en/stable/index.html) - Voilà allows you to convert a Jupyter Notebook into an interactive dashboard that allows you to share your work with others.

* [Aeris_Weather_API](https://github.com/aerisweather/python-tools) - the AerisWeather API give users the ability to download weather data and load into a pandas DataFrame for data science purposes.
---

## Installation Guide

### Before running the application first install the following dependencies in either Gitbash or Terminal. (If not already installed)

#### Step1: Activate dev environment in Gitbash or Terminal to do so type:
```python
    conda activate dev
```
#### Step2: install the following libraries (if not installed yet) by typing:
```python
    pip install pandas
    pip install numpy
    pip install SQLAlchemy
    pip install python-dotenv
    pip install -U scikit-learn
    conda install -c anaconda requests
    conda install -c jmcmurray json    
    conda install -c pyviz hvplot
    conda install -c conda-forge voila

    
```
#### Step3: Start Jupyter Lab
Jupyter Lab can be started by:
1. Activate your developer environment in Terminal or Git Bash (already done in step 1)
2. Type "jupyter lab --ContentsManager.allow_hidden=True" press enter (This will open Jupyter Lab in a mode where you can also see hidden files)

![JupyterLab](https://github.com/vincentsgarzi/Group5Project1/blob/main/Images/JupyterLab.PNG)


## Usage

To use the Personal Energy Usage Analysis jupyter lab notebook, simply clone the full repository and open the **Personal_Energy_Usage_Final_2022_per_hr.ipynb** file in Jupyter Lab. 

The tool will go through the following steps:

### Analysis household's historical energy usage and relationship between historical energy usage and historical temperature data
* Analyze a household's historical energy usage and calculated the regression between temperature and energy usage

### Calculated correlation between price of energy in kWh and natural gas and Crude Oil
* Analyze what energy product is most correlated with the price of kWh in the state of NY. 

### Predict the future price of the most correlated driver of kWh price in the state of NY
* Analyze the performace of the most correlated product in a monte carlo simulation to predict the future price of kWh in the state of NY. 

### Instructions on how to deploy the notebook as a web application using VOILA library
* Last are instructions on how to deploy the notebook as a web application (Please also see below example). 

![Voila_Screenshot_and_Terminal.jpg](https://github.com/vincentsgarzi/Group5Project1/blob/main/Images/Voila_Screenshot_and_Terminal.jpg)

## Contributor(s)

This project was created by Columbia Fintech Group 5:
Andre Johnson
Marc Pocorni
Vincent Sgarzi
Niels de Haan

---

## License(s)

MIT
