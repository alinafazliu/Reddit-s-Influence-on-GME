# Reddit-s-Influence-on-GME
A Machine Learning Project that analyses Reddit's influence on GameStop

### Install

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [dateutil](https://pypi.org/project/python-dateutil/)
- [xgboost](https://pypi.org/project/xgboost/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://jupyter.org/install.html).

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](https://www.anaconda.com/download/) distribution of Python, which already has the above packages and more included. 

### Code

The data preprocessing code is provided in the `Reddit_GME.ipynb` notebook file. In order to find the best model possible for this project, there have been used four models. Linear Regression model is in the `Linear Regression.ipynb` file. Xgboost's model of Linear Regression is on the `xgb Linear Regression.ipynb`, while xgboost's Random Forest Regressor is on `xgb RFRegressor.ipynb` file. The simple Random Forest Regressor is on the `Random Forest Regressor.ipynb` file.

### Run

To start one of the notebooks run one of the following commands:

```bash
ipython notebook <filename>.ipynb
```  
or
```bash
jupyter notebook <filename>.ipynb
```
or open with Jupyter Lab
```bash
jupyter lab
```

This will open the Jupyter Notebook software and project file in your browser.

As an alternative you can also use Google's colaboratory service to open the notebooks on the web  
[Google colaboratory](https://colab.research.google.com/?utm_source=scs-index)

### Data
The Reddit dataset has been merged with the Gamestop stock dataset in an hour to hour basis. The dataset consists of 1369 data points, with each datapoint having 3 features. This dataset has been created by scraping Reddit through the [pushshift API](https://pushshift.io/). The Gamestop hourly data was scraped by the open stock API provided by [alphavantage](https://www.alphavantage.co/).

**Features**
1.  `score`: the score of the Reddit posts
2. `comms_num`: number of comments on Reddit posts
3. `mentioned`: How many times was Gamestop mentioned on posts

**Target Variable**
4. `close`: closing stock value of Gamestop