#election

###Contributors
+ Jun Seo Park
+ Athan Diep
+ Emma Duncan

##Abstract
The 2016 U.S. presidential election yielded an unexpected result for many - while an overwhelming majority of polls were thought to point to Hillary Clinton as the winner, Donald Trump emerged the victor. In this project, we dive into the election poll data provided by [FiveThirtyEight](https://projects.fivethirtyeight.com/2016-election-forecast/) with the goal of visualizing the data to see where the predictions may have gone awry. **include link/description to markdown file for presentation**

##IPython notebooks
There are two IPython notebooks: [Election 2016 (Bokeh).ipynb](../blob/master/Election 2016 (Bokeh).ipynb) and pElection 2016 (Plotly).ipynb](../blob/master/Election 2016 (Plotly).ipynb).
+ Election 2016 (Bokeh) was the initial iteration, built upon the data visualization package [Bokeh](http://bokeh.pydata.org/en/latest/#). Though Bokeh is a beautiful package with straightforward syntax, we ran into some major roadblocks with the lack of documentation and crucial missing features.
+ Election 2016 (Plotly) is the current iterattion, using the data visualization package [Plotly](https://plot.ly). Plotly has a variety of available charts, complete with [detailed documentation for Python](https://plot.ly/python/).

##System requirements
This project was built on virtual environments running Python 3.6 through Anaconda, and we have also included two separate requirements.txt files for [Windows](..blob/master/requirements_windows.txt) and [OSX/macOS](..blob/master/requirements_mac.txt).
To create a virtual environment, enter the following in a command-line interpreter (Anaconda Prompt, Terminal, etc.):
```python
conda create python=3.6 --name [envname] --file [filepath]
```
+ filepath refers to the path of the respective requirements.txt file.
To activate the environment on Windows:
```python
activate [envname]
```
And on OSX/macOS:
```python
source activate [envname]
```
Jupyter notebooks can be opened using the command:
```python
jupyter notebook
```
And virtual environments can be closed by (preceded by `source` on OSX/macOS):
```python
deactivate [envname]
```
For more information regarding virtual environments, reference the [official Conda documentation](https://conda.io/docs/using/envs.html).