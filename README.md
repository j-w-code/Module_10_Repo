# *Crypto Investments*
---

## Crypto Investments
This project covers the use of the SKlearn libraries such as "cluster", "decomposition", and "preprocessing" to perform unsupervised learning on datasets. The results are then used to cluster data for inerpretation.  

>"In my defense, I was left unsupervised"

## Technologies 

This project uses Pandas, Hvplot, and SKLearn libraries to create dataframes, perform unsupervised machine learning, and plot graphical interpretations of data. 

[pandas](https://github.com/pandas-dev/pandas)
[HVplot](https://github.com/holoviz/hvplot)
[SKLearn](https://github.com/scikit-learn/scikit-learn)

### Installation Guide

In order to use this program please import and utilize the following libraries and dependencies: 

```python
import pandas as pd
import hvplot.pandas
from pathlib import Path
from sklearn.cluster import KMeans
from sklearn.decomposition import PCA
from sklearn.preprocessing import StandardScaler
```

## Usage 
the following blocks of code from the Pandas library are fundamental in executing the program. 

```python 
StandardScaler().fit_transform()
```
This normalizes the data to fit our machine learning algorithms. 
```python
columns=df.columns
```
This command allows us to set the columns of a dataframe to be equal to that of a previously constructed dataframe.  
```python
model = KMeans(n_clusters=, random_state=)
```
This command sets the initial machine learning model from SKlearn. The number of clusters is variable as is the random state.  
```python
model.fit(df)
```
This command fits a dataframe to the previoulsy specified KMeans model (see above code).   
```python
clusters = model.predict(df)
```
this command will use the transformed historical data to make predictions based on the unsupervised learning algorithm. It will then output data for further interpretations. 

```python
df.hvplot.scatter(x="",y="", hover_cols="", by="")
```

This plot command will display the data in a scatter formation along the specified axis criteria.                 

![<alt text>](https://i.postimg.cc/KcnNCHyw/Screen-Shot-2022-06-23-at-10-48-09-AM.png)

## Contributors

Jeffrey J. Wiley Jr

## License

MIT


