In this assignment you will practice writing backpropagation code, and training
Neural Networks and Convolutional Neural Networks. The goals of this assignment
are as follows:

- understand **Neural Networks** and how they are arranged in layered
  architectures
- understand and be able to implement (vectorized) **backpropagation**
- implement various **update rules** used to optimize Neural Networks
- implement **batch normalization** for training deep networks
- implement **dropout** to regularize networks
- effectively **cross-validate** and find the best hyperparameters for Neural
  Network architecture
- understand the architecture of **Convolutional Neural Networks**
- gain an understanding of how a modern deep learning library (PyTorch) works
  and gain practical experience using it to train models.

## Setup
Make sure your machine is set up with the assignment dependencies. 
You will need to make your own requirements.txt as well for your enviornment. You should keep minimal amount of libraries in your file.~ 

**[Option 1] Use Anaconda:**
[Anaconda](https://www.continuum.io/downloads) is a Python distribution
that includes many of the most popular Python packages for science, math,
engineering and data analysis. 

**[Option 2] Manual install, virtual environment:**
If you do not want to use Anaconda and want to go with a more manual
installation route you will likely want to create a
[virtual environment](http://docs.python-guide.org/en/latest/dev/virtualenvs/)
for the project. To set up a virtual environment, run the following:

```bash
cd assignment1
sudo pip install virtualenv      # This may already be installed
virtualenv .env                  # Create a virtual environment
source .env/bin/activate         # Activate the virtual environment
pip install -r requirements.txt  # Install dependencies
# Work on the assignment for a while ...
deactivate                       # Exit the virtual environment
```

**Download data:**
Once you have the starter code, you will need to download the CIFAR-10 dataset.
Run the following from the `assignment1` directory:

```bash
cd deeplearning/datasets
./get_datasets.sh
```

If you are on Mac, this script may not work if you do not have the wget command 
installed, but you can use curl instead with the alternative script.
```bash
cd deeplearning/datasets
./get_datasets_curl.sh
```

### Submitting your work:
You will need to create a private fork of this repository and add your SME as a collaborator to the repoistory.

### Q1: Fully-connected Neural Network
The IPython notebook `FullyConnectedNets.ipynb` will introduce you to our
modular layer design, and then use those layers to implement fully-connected
networks of arbitrary depth. To optimize these models you will implement several
popular update rules.

### Q2: Batch Normalization
In the IPython notebook `BatchNormalization.ipynb` you will implement batch
normalization, and use it to train deep fully-connected networks.

### Q3: Dropout
The IPython notebook `Dropout.ipynb` will help you implement Dropout and explore
its effects on model generalization.

### Q5: Train a model on CIFAR10 using Pytorch! (10 points) 
Now that you've implemented and gained an understanding for many key components 
of a basic deep learning library, it is time to move on to a modern deep learning
library: Pytorch. Here, we will walk you through the key concepts of PyTorch, and
you will use it to experiment and train a model on CIFAR10. We highly recommend 
you use Google Colab (https://colab.research.google.com/) for this notebook, as it
comes with Pytorch installed and provides access to GPUs.

If you use Colab for this notebook, make sure to manually download the completed 
notebook and place it in the assignment directory before submitting. Also remember 
to download required output file and place it into submission_logs/ directory.


