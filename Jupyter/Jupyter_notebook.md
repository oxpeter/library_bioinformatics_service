![Weill Cornell Medicine Samuel J. Wood Library](../images/WCM_SamWoodLib.png)


# Jupyter Notebook Tutorial
## A tutorial to install and run Jupyter notebooks


```
Peter Oxley, PhD
Associate Director of Research Services

Weill Cornell Medicine
Information Technologies and Services
Samuel J. Wood Library & C.V. Starr Biomedical Information Center
1300 York Avenue Room D-120
New York, NY 10065-4896
(P) 646-962-2576
(F) 212-746-8364
 
pro2004@med.cornell.edu
```

![Library Bioinformatic Service](../images/LBS.png)


## Installing and starting the notebook
### Installing jupyter notebook
__For non-experienced users__
1) download and install [Anaconda](https://www.continuum.io/downloads)

_Anaconda provides a user-friendly graphical interface to manage environments, scientific computing packages, and the Jupyter notebook._

__For experienced python users__

```
pip3 install --upgrade pip
pip3 install jupyter
```

_This method leaves the management of virtual environments, upgrades and installation of packages to the user via other means (most commonly, through the command line)._


### Starting a notebook server
1) Activate your appropriate environment.
2) If using Anaconda, open the application, then click on "Launch" in the Jupyter notebook panel. Alternatively, enter  ```jupyter notebook``` in the terminal. 
3) Your default browser should open to a new tab and open the notebook dashboard. The URL is printed in the terminal window when the notebook starts. The default is ```http://localhost:8888```.

_More details and options can be found in the [Jupyter documentation](https://jupyter.readthedocs.io/en/latest/running.html#running)_

## Exercise A) Create a new notebook
1) From the dashboard, navigate to the folder in which you would like to create your notebook. Clicking on a folder name will open the folder and display its contents. You can create a new folder by selecting  ```New ▼ > Folder``` from the button on the right, above the file list. 
2) Create a new notebook by selecting ```New ▼ > ```  and choosing the kernel you wish to use. The basic installation will only have the IPython kernel available. However, you can install additional kernels to access other languages from the notebook (See exercise J).

 



## Exercise B) Using R in Jupyter notebooks
__Install R-essentials and rpy2__
This first requires that you have R installed on your computer.
In the terminal, enter:

```
conda install -c r r-essentials
conda install -c r rpy2
```

_This will include the installation of the packages dplyr, shiny, ggplot2, tidyr, caret, and nnet._


## Exercise C) Installing a kernel for working in R
_There are more than 80 different kernels available for Jupyter, giving access to many languages, including [Java, Matlab, Octave, bash, C#, C++, Julia, Jython, scala, etc](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels). Installation of these can vary from the example given here, so you will need to check the instructions for each one you wish to add to your Jupyter kernel repertoire_ 

1) Make sure you have R installed
2) In the terminal, start R (do not use R-Studio for the following steps):

```
$ R
> install.packages(c('repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))
> devtools::install_github('IRkernel/IRkernel')
> IRkernel::installspec()
```


![LBS](../images/motif.png)

----------