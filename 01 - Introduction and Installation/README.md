# Installation

## Working on your local machines
Linux and Mac OS comes with pre-installed Python. To run python, open terminal and type:
```
python3
```
Windows users can download python from [here](https://www.python.org/downloads/)

If you wish to work locally on your machines, it is recommended to use a virtual environment.

### Why virtual environment instead of system Python?
Running with the system Python and libraries limits you to one specific Python version, chosen by your OS provider. Trying to run all Python applications on one Python installation makes it likely that version conflicts will occur among the collection of libraries. It's also possible that changes to the system Python will break other OS features that depend on it.

Virtual environments, or "virtualenvs" are lightweight, self-contained Python installations, designed to be set up with a minimum of fuss, and to "just work" without requiring extensive configuration or specialized knowledge.

virtualenv avoids the need to install Python packages globally. When a virtualenv is active, you will install packages within the environment, which does not affect the base Python installation in any way. Thus, allowing you to have isloated version of packages for each project you are working on.

### Anaconda Virtual Environment
It is strongly recommended using the free Anaconda Python distribution, which provides an easy way for you to handle package dependencies. 
You can download it from [here](https://www.anaconda.com/products/individual#Downloads)

Once you are done with installing anaconda, the next step is to create a virtual environment for you project.
To setup a virtual environment (lets name it "myenv")
```
# this will create environment at location path/to/anaconda3/envs/ with specific version of python
conda create --name myenv myenv python=3.7
```
To activate enter command `activate myenv` and `deactivate` to simply return to base environment or exit the terminal.

some useful commands in anaconda are:
```
# display lists of environments
conda info --envs

# install pip in anaconda, pip is useful for installing python packages
conda install pip

# for example to install opencv
pip install opencv-python

# To run jupyter notebook from anaconda enter following command in your project directory
jupyter notebook
```
# Working remotely
Google Colaboratory is basically a combination of Jupyter notebook and Google Drive. It runs entirely in the cloud and comes preinstalled with many packages (e.g. OpenCV and NumPy) so everyone has access to the same dependencies. Even cooler is the fact that Colab benefits from free access to hardware accelerators like GPUs (K80, P100) and TPUs.

## Requirements
You must have google account linked with google drive.

Go to https://colab.research.google.com/ and create a new notebook

Now, to confirm your installation you can run a "Hello World" program on any of these setups.
```
print("Hello World")
# Outputs Hello World
```
