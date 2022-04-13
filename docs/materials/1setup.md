# Setting up PyTorch

Installing PyTorch on your own computer should be quite straightforward. 
The recommended way is to install it using an Anaconda environment. 
There are instructions here: https://pytorch.org/get-started/locally/

If you run into problems which are difficult to solve, you can also use Google Colaboratory: https://colab.research.google.com/notebooks/welcome.ipynb It can be set up to install PyTorch. See the instructions below.

You should use a 3.x version of Python since Python 2 is not supported anymore.
Through Anaconda, it is straightforward to install PyTorch and other libraries. 
You can also start Jupyter Notebooks from its interface. 

# Setting up Jupyter Notebooks

(If you're new to Jupiter Notebooks, we recommend this link: https://www.dataquest.io/blog/jupyter-notebook-tutorial/)

You can install Jupyter Notebooks via conda or pip. Find the instructions here: https://jupyter.org/install

1. Setting up Jupyter Notebooks to work with conda environments:

Since conda has stopped automatically setting environments up as jupyter
kernels, you need to either manually add them, or install the nb_conda_kernels
package which does the setting up for you. Below are instructions to set up using the nb_conda_kernels package. For manual set up, you can refer to this stackoverflow post: https://stackoverflow.com/questions/39604271/conda-environments-not-showing-up-in-jupyter-notebook

Using nb_conda_kernels package:

(You can find the complete instructions and explanations for installing this package here: https://github.com/Anaconda-Platform/nb_conda_kernels)

First, you need to install nb_conda_kernels package to the environment from which you run Jupyter Notebook. This might be your base conda environment, 

$ conda install nb_conda_kernels

but it need not be. For instance, if the environment notebook_env contains the notebook package, then you would run:

$ conda install -n notebook_env nb_conda_kernels

In addition, if your pytorch environment (which you are using for this project) and the notebook_env (the environment from which you will run jupyter notebooks) are different, then in the pytorch environment you should also install the ipykernel package. Say, if it is called pytorch_env:

$ conda install nb_conda_kernels

or 

$ conda install -n pytorch_env ipykernel


