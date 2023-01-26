# Fintech_Module7


![ETF_Returns_Analyzer.jpg](https://github.com/nielsdehaan1977/Fintech_Module7/blob/main/Images/ETF_Returns_Analyzer.jpg)

## ETF Analysis, a financial database and web application that uses SQL, Python, and the Voilà library to analyze the performance of an ETF and its indivual components.

## etf_analyzer.ipynb
---

### This Jupyter notebook can be used as a template for ETF analysis, it utilizes SQL, Python and results can be displayed webbased via Viola library

The tool can help with analyzing single asset and can analyze the full ETF portofolio. 
* Anaylsis is done on the following steps: 
1. Analysis of a single asset in an ETF
2. Optimization of data accessiblity with the use of SQL queries
3. Analysis of the full ETF portfolio
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

* [hvplot](https://hvplot.holoviz.org/user_guide/Plotting.html) - hvplot is generate plots from Pandas DataFrames and many other data structures of the PyData ecosystem.

* [sqlalchemy](https://www.sqlalchemy.org/) - SQLAlchemy is a Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL.

* [voila](https://voila.readthedocs.io/en/stable/index.html) - Voilà allows you to convert a Jupyter Notebook into an interactive dashboard that allows you to share your work with others.
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
    conda install -c pyviz hvplot
    conda install -c conda-forge voila  
    
```
#### Step3: Start Jupyter Lab
Jupyter Lab can be started by:
1. Activate your developer environment in Terminal or Git Bash (already done in step 1)
2. Type "jupyter lab --ContentsManager.allow_hidden=True" press enter (This will open Jupyter Lab in a mode where you can also see hidden files)

![JupyterLab](https://github.com/nielsdehaan1977/Fintech_Module7/blob/main/Images/JupyterLab.PNG)


## Usage

To use the etf analyzer jupyter lab notebook, simply clone the full repository and open the **etf_analyzer.ipynb** file in Jupyter Lab. 

The tool will go through the following steps:

### Analysis of a single asset in an ETF
* Analyze a single asset in the ETF. 

### Optimization of data accessiblity with the use of SQL queries
* SQL queries are used to optimize the efficiency of accessing the available data from the database.

### Analysis of the full ETF portfolio
* Analyze the entire ETF portfolio and evaluate its performance. Tool builds the entire ETF portfolio by using SQL joins to combine all the data for each asset.

### Instructions on how to deploy the notebook as a web application using VOILA library
* Last are instructions on how to deploy the notebook as a web application (Please also see below example). 

![Voila_Screenshot_and_Terminal.jpg](https://github.com/nielsdehaan1977/Fintech_Module7/blob/main/Images/Voila_Screenshot_and_Terminal.jpg)

## Contributor(s)

This project was created by Niels de Haan (nlsdhn@gmail.com)

---

## License(s)

MIT
