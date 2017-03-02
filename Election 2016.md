# Election 2016: An Exploratory Data Analysis

## Table of Contents
1. Environment Setup
2. Loading Data
3. Scatter Plots
4. Box Plot
5. Line Graph with Error Bars
6. Bubble Chart
7. Chloropleth Maps





## Environment Setup
### Anaconda & Virtual Environment
This project was built on an [Anaconda](https://www.continuum.io/downloads) virtual environment running Python 3.6. Install Anaconda, and download the correct requirements file ([Windows](../master/requirements_windows.txt) or [OS X/macOS](../master/requirements_mac.txt)). Open Anaconda Prompt (Windows) or Terminal (OS X/macOS), and enter the following:
```sh
conda create python=3.6 --name [envname] --file [filepath]
```
+ `[envname]` will be the name of your environment.
+ `[filepath]` is the path to your downloaded requirements file.

Once that finishes, you're ready to activate your new virtual environment! For Windows:
```sh
activate [envname]
```
And for OS X/macOS:
```sh
source activate [envname]
```

Jupyter notebooks allow you to run snippets of your code and see results on the spot. Open Jupyter notebooks using the command:
```sh
jupyter notebook
```
A cheat sheet for keyboard shortcuts can be found [here](https://zenodo.org/record/44973/files/ipynb-cheat-sheet.pdf).

And once you're finished working, virtual environments can be closed in command line by (preceded by `source` on OS X/macOS):
```sh
deactivate [envname]
```

### Plotly
Plotly for Python requires an account and an API key, both of which are available on the free tier plan. Though the free tier plan is limited to 250 API calls per day, it offers access to the same amenities as the paid tiers. Once an account has been made and an API key has been generated, Plotly can be activated within the script using the code:
```python
import plotly.plotly as py
py.sign_in('username', 'api_key')
```
For privacy reasons, we have executed then deleted this line from our Jupyter notebooks. Please follow these steps in order to recreate Plotly visualizations in your notebook.

Awesome! Let's get started.





## Loading Data
We start off by loading the packages that we want to use.
```python
import numpy as np
import pandas as pd
import plotly.plotly as py
import plotly.graph_objs as go
from plotly import tools
pd.set_option('display.max_columns', 100) #overrides default to display up to 100 columns in dataframes
```