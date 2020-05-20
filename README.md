# Bike-Sharing-Prediction-with-NeuralNet

Developed as coursework for Udacity "Deep Learning Fundamentals" Nanodegree. In this project, I built a neural network to predict daily bike rental ridership.

## Further Explanation

The Neural network was built from "scratch", using only NumPy to assist. The goal of this project is to understand what happens behind the neural network before diving deeper into other tools like TensorFlow.

## Results

The project meets the specifications, which are:

All the code in the notebook runs in Python 3 without failing, and all unit tests pass.

The sigmoid activation function is implemented correctly

The forward pass is correctly implemented for the network's training.

The run method correctly produces the desired regression output for the neural network.

The network correctly implements the backward pass for each batch, correctly updating the weight change.

Updates to both the input-to-hidden and hidden-to-output weights are implemented correctly.

The number of epochs is chosen such the network is trained well enough to accurately make predictions but is not overfitting to the training data.

The number of hidden units is chosen such that the network is able to accurately predict the number of bike riders, is able to generalize, and is not overfitting.

The learning rate is chosen such that the network successfully converges, but is still time efficient.

The number of output nodes is properly selected to solve the desired problem.

The training loss is below 0.09 and the validation loss is below 0.18.

## Conclusion

The predictions given by the model are quite accurate. However, the model overestimes bike ridership in December because it hasn't had sufficient holiday season training examples.

# Dependencies

## Configure and Manage Your Environment with Anaconda

Per the Anaconda [docs](http://conda.pydata.org/docs):

> Conda is an open source package management system and environment management system 

for installing multiple versions of software packages and their dependencies and 

switching easily between them. It works on Linux, OS X and Windows, and was created 

for Python programs but can package and distribute any software.

## Overview

Using Anaconda consists of the following:

1. Install [`miniconda`](http://conda.pydata.org/miniconda.html) on your computer, by selecting the latest Python version for your operating system. If you already have `conda` or `miniconda` installed, you should be able to skip this step and move on to step 2.

2. Create and activate * a new `conda` [environment](http://conda.pydata.org/docs/using/envs.html).

\* Each time you wish to work on any exercises, activate your `conda` environment!

---

## 1. Installation

**Download** the latest version of `miniconda` that matches your system.

|        | Linux | Mac | Windows | 

|--------|-------|-----|---------|

| 64-bit | [64-bit (bash installer)][lin64] | [64-bit (bash installer)][mac64] | [64-bit (exe installer)][win64]

| 32-bit | [32-bit (bash installer)][lin32] |  | [32-bit (exe installer)][win32]

[win64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe

[win32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86.exe

[mac64]: https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh

[lin64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh

[lin32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86.sh

**Install** [miniconda](http://conda.pydata.org/miniconda.html) on your machine. Detailed instructions:

- **Linux:** http://conda.pydata.org/docs/install/quick.html#linux-miniconda-install

- **Mac:** http://conda.pydata.org/docs/install/quick.html#os-x-miniconda-install

- **Windows:** http://conda.pydata.org/docs/install/quick.html#windows-miniconda-install

## 2. Create and Activate the Environment

For Windows users, these following commands need to be executed from the **Anaconda prompt** as opposed to a Windows terminal window. For Mac, a normal terminal window will work. 

#### Git and version control

These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:

```

conda install git

```

If you'd like to learn more about version control and using `git` from the command line, take a look at our [free course: Version Control with Git](https://www.udacity.com/course/version-control-with-git--ud123).

**Now, you're ready to create your local environment!**

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.

```

https://github.com/subhayu99/bike_sharing_project_with_NN.git

cd bike_sharing_project_with_NN

```

2. Create (and activate) a new environment, named `deep-learning` with Python 3.6. If prompted to proceed with the install `(Proceed [y]/n)` type y.

	- __Linux__ or __Mac__: 

	```

	conda create -n deep-learning python=3.6

	source activate deep-learning

	```

	- __Windows__: 

	```

	conda create --name deep-learning python=3.6

	activate deep-learning

	```

		At this point your command line should look something like: `(deep-learning) <User>:deep-learning-v2-pytorch <user>$`. The `(deep-learning)` indicates that your environment has been activated, and you can proceed with further package installations.

3. Install PyTorch and torchvision; this should install the latest version of PyTorch.

	

	- __Linux__ or __Mac__: 

	```

	conda install pytorch torchvision -c pytorch 

	```

	- __Windows__: 

	```

	conda install pytorch -c pytorch

	pip install torchvision

	```

6. Install a few required pip packages, which are specified in the requirements text file (including OpenCV).

```

pip install -r requirements.txt

```

7. That's it!





```

cd

cd bike_sharing_project_with_NN


jupyter notebook

```

To exit the environment when you have completed your work session, simply close the terminal window.
