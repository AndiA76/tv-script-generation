# TV Script Generation using RNNs and Pytorch

## Overview

This project from Udacity's nano-degree course "Deep-Learning" is about TV Script Generation using a Recurrent Neural Network (RNN) - in this case based on Long Short-Term Memory (LSTM) Cells. The task is to set up an RNN, which is trained on [Seinfield](https://en.wikipedia.org/wiki/Seinfeld) TV scripts. The goal is to artificially generate new "fake" TV scripts that are similar to the original ones based on patterns that are learned from the original TV scripts.

The project is broken down in subtasks starting with loading, exploring and preprocessing the TV script data, analysing the vocabulary, defining the recurrent neural network model (incl. vocabulary embedding, definition of loss and optimization criteria), training the RNN model and finally evaulating the performance by artificially generating a new "fake" TV script.

The project is implemented as a Jupyter notebook and can be found there: [Project Notebook](dlnd_tv_script_generation.ipynb)

## Installation

### 1. Install Anaconda with Python

In order to run the notebook please download and install [Anaconda](https://docs.anaconda.com/anaconda/install/) with Python 3.6 on your machine. Further packages that are required to run the notebook are installed in a virtual environment using conda.

### 2. Create a Virtual Environment

In order to set upt the prerequisites to run the project notebook you should create a virtual environment, e. g. using conda, Anaconda's package manager, and the following command

```
conda create --name deep-learning
```

The virtual environment needs to be activated by

```
activate deep-learning
```

### 3. Download the project from github

You can download the project from github as a zip file to your Downloads folder from where you can unpack and move the files to your local project folder. Or you can clone from Github using the terminal window. Therefore, you need to prior install git on your machine e. g. using

```
conda install -c anaconda git
```

When git is installed you can create your local project version. Therefore, navigate to your project folder and clone the project from github using the command

```
git clone https://github.com/AndiA76/tv-script-generation.git
```

Then change to the project directory

```
cd tv-script-generation
```

### 4. Install Pytorch with GPU support

In order to run the project notebook you need to install Pytorch. If you wish to install Pytorch with GPU support you also need to take care of your CUDA version and some [dependencies with Pytorch](https://pytorch.org/get-started/previous-versions/). I have used Ubuntu 18.04 LTS with CUDA 10.0 and Python 3.6 to run the project notebook. Therefore you need to enter the following installation command:

CUDA 10.0
```
conda install pytorch==1.2.0 torchvision==0.4.0 cudatoolkit=10.0 -c pytorch
```

### 5. Further requirements 

Besides Pytorch you need to install a couple of further packages, which are required by the project notebook. The packages are specified in the [requirements.txt](requirements.txt) file (incl. OpenCV for Python). You can install them using pip resp. pip3:

```
pip install -r requirements.txt
```

### 6. Download the dataset

In this project, you'll be using a part of the Seinfeld dataset of scripts from 9 seasons of the TV series. The dataset is already provided in the repository for you in ./data/Seinfeld_Scripts.txt.

### 7. Run the notebook

Now start a Jupyter notebook to run the project using following command

```
jupyter notebook
```

Navigate to your local project folder in the Jupyter notebook and open [dlnd_tv_script_generation.ipynb](dlnd_tv_script_generation.ipynb) file and run it.
