# election

### Contributors
+ Jun Seo Park
+ Athan Diep
+ Emma Duncan

## Abstract
The 2016 U.S. presidential election yielded an unexpected result for many - while an overwhelming majority of polls were thought to point to Hillary Clinton as the winner, Donald Trump emerged the victor. In this project, we dive into the election poll data provided by [FiveThirtyEight](https://projects.fivethirtyeight.com/2016-election-forecast/) with the goal of visualizing the data to see where the predictions may have gone awry. 
+ We used IPython notebooks to write our script, and the final product can be found on [Election 2016.ipynb](../master/Election 2016.ipynb). More information about the two IPython notebooks can be found below.
+ We have included both a .zip and .csv of the election poll data in the repository. If you wish to download or import the dataset using a link, it is available at [http://projects.fivethirtyeight.com/general-model/president_general_polls_2016.csv](http://projects.fivethirtyeight.com/general-model/president_general_polls_2016.csv).

## IPython notebooks
There are three IPython notebooks in this repository: [Election 2016 (Bokeh)](../master/Election 2016 (Bokeh).ipynb) and [Election 2016 (Plotly)](../master/Election 2016 (Plotly).ipynb), and [Election 2016](../master/Election 2016.ipynb).
+ Election 2016 (Bokeh) was the initial iteration, built upon the data visualization package [Bokeh](http://bokeh.pydata.org/en/latest/#). Though Bokeh is a beautiful package with straightforward syntax, we ran into some major roadblocks with the lack of documentation and crucial missing features.
+ Election 2016 (Plotly) is the code for the current iteration, using the data visualization package [Plotly](https://plot.ly). Plotly supports a variety of chart types, complete with [detailed documentation for Python](https://plot.ly/python/). If you are interested in porting the project into another language, Plotly also supports R, Matlab, and Excel, among others.
+ The final presentation of the project is available on Election 2016. It includes explanations for data visualization, and the process through which the dataset was cleaned.

## System requirements
### Anaconda Virtual Environments
This project was built on virtual environments running Python 3.6 through Anaconda, and we have also included two separate requirements.txt files for [Windows](..blob/master/requirements_windows.txt) and [OS X/macOS](..blob/master/requirements_mac.txt).
To create a virtual environment, enter the following in a command-line interpreter (Anaconda Prompt, Terminal, etc.):
```sh
conda create python=3.6 --name [envname] --file [filepath]
```
+ filepath refers to the path of the respective requirements.txt file.

To activate the environment on Windows:
```sh
activate [envname]
```
And on OS X/macOS:
```sh
source activate [envname]
```
Jupyter notebooks can be opened using the command:
```sh
jupyter notebook
```
And virtual environments can be closed by (preceded by `source` on OS X/macOS):
```sh
deactivate [envname]
```
For more information regarding virtual environments, reference the [official Conda documentation](https://conda.io/docs/using/envs.html).

### Plotly
Plotly for Python requires an account and an API key, both of which are available on the free tier plan. Though the free tier plan is limited to 250 API calls per day, it offers access to the same amenities as paid tiers.
Once an account has been made and an API key has been acquired, Plotly can be activated within the script using the code:
```python
import plotly.plotly as py
py.sign_in('username', 'api_key')
```
For privacy reasons, we have executed then deleted this line from our Jupyter notebooks. Please follow these steps in order to recreate Plotly visualizations.
