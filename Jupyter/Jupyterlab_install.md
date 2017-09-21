# Instructions for installation and configuration of Jupyterlab

These instructions form a quick and simple setup to get Jupyterlab running via Anaconda.

## Install software
1. Visit (anaconda.org)[anaconda.org]
2. Download and install Anaconda
3. Visit (nodejs.org )[nodejs.org]
4. Download and install nodejs

## Setup environment
5. Open Anaconda
6. Click on "Environments" tab on left panel
7. Click on "Create" at bottom of middle panel to create new environment
8. Give new environment a name and select python3 (and any additional choices)
9. Select "Chanels" in the top of the right-hand panel
10. Select "Add..." in the top right corner
11. Enter `conda-forge` and hit enter.
12. Click "Update channels" and then close the window.
13. Select "All" from the dropdown menu in the top of the right-hand panel.
14. Click "Update index"
14. Enter `jupyterlab` in the textbox to the right.
15. Select "jupyterlab" from the options.
16. Click "Apply" in the bottom right corner.
17. A window will pop up showing the updates that will be made. Select "Accept" to install jupyterlab.
18. Repeat from step 11 to add any additional libraries (eg pandas, scipy, scikit-learn)

## Install google-drive extension
1. in terminal, ensure that anaconda/bin is included in your path:

    `eg. export PATH="/User/Guest/anaconda/bin:$PATH`


2. activate the environment created above:

    `source activate <envt_name>`


3. install (google-drive)[https://github.com/jupyterlab/jupyterlab-google-drive] extension :

    `jupyter labextension install @jupyterlab/google-drive`


## Launch JupyterLab server
1. In terminal, enter:

    `jupyter lab`
    
## ipywidgets
```
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```

## Jupyterlab renderers
* plotly
* json
* geojson

https://github.com/jupyterlab/jupyter-renderers