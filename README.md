# 26 week Machine Learning and Artificial Intelligence course

Hello and welcome to my 26 week ML and AI course. This course is designed for year 12 students (or 11th grade US students), who have some familiarity with calculus/pre-calculus and basic coding principles. 

The goal of this course is to start from the fundamentals of linear algebra, probability theory and multivariate calculus and eventually build up to implementing and training your own neural networks by the end of the course. The course finishes with a 3-4 week capstone project where you can sort of do whatever you like, but you are perfectly free to spend longer.  

Materials will be released each week from my private repository for you to have a go at, this includes both lecture notes/slides and some programming exercises in Python. Don't worry if you fall a bit behind we probably won't rigorously stick to the schedule and can spend more time on trickier things. 

## Video materials for linear algebra

[3Blue1Brown essence of linear algebra](https://youtu.be/kjBOesZCoqc?si=UUkI12_ND45JzhCQ)

## Machine learning with Python

Check out scitkit-learn a machine learning toolbox that implements various classical ML algorithms, for regression, classification and unsupervised learning.

[Scitkit-learn](https://scikit-learn.org/stable/)

## Getting started with coding

If you have yet to install Anaconda and Python please see **Installing and setup instructions** below.

If you have everything set up open your terminal (Mac), cmd (Windows), or Debian/Ubuntu (Linux) navigate to your coding directory with ```cd``` and ```ls``` (Max/Linux) or ```dir``` e.g.

```cd tech_elective```

```conda activate ml```

```jupyter notebook```

To move up a directory:

```cd ..```

## Accessing resources through google colab

If you don't have python or Anaconda installed you can still access the resources through google colab. 

Go to [Google Colab](https://colab.research.google.com/)

```File -> Open Notebook```

Click GitHub and then search my username: sacktock

Choose the repository 26-week-Ml-public and then choose which notebook to open.

## Course overview

Week 1: Introduction to the course, setup and basic Python programming

Week 2: Fundamentals of linear algebra, vector spaces, multiplication, transposition, linear transformations, matrix inverse, determinant, eigenvalues, eigenvectors.

Week 3: Basics of multivariate calculus, funtions of multiple variables, partial derivatives, vectorized gradients, critical points, Hessian matrix, Jacobians, simple linear regression, least squares estimate.

Week 4: Linear regression in depth, multiple linear regression, derivation of the least squares estimate for the multivariate case, 

Week 5: Introduction to classification, logistic regression, performance metrics (precision, recall F-1 score).

Week 6: Polynomial basis expansion, bias-variance tradeoff, lasso and ridge regression logistic regression with L2 and L1 regulzarization, 

Week 7: Unsupervised learning, K-means clustering, PCA and SVD.

Week 8: Introduction to neural networks, neurons, activation functions, feed forward neural networks, forward equations.

Week 9: Introduction to feedforward neural networks designing neural network architectures, loss functions and optimization algorithms (SGD, SGD with momentum, Adam), learning rates and epochs.

Week 10: Advanced topics with neural networks, regularization techniques, dropout, batch norm, weight decay, model evaluation and overfitting.

Week 11: Introduction to convolutional neural networks, convolutions, pooling layers, hands on implementation details.

Week 12: Introduction to recurrent neural networks, time series forcasting and sequential data, vanishing gradient problem, LSTM and GRU.

Week 13: Introduction to reinforcement learning, agents, states, actions, rewards, Q learning and deep Q learning, applications.

Week 14-26: Capstone project based on any of the main topics introduced throughout the course.

## Installation and setup instructions

Please install conda via [Anaconda](https://www.anaconda.com/download/success) and make sure you install the correct distribution for your machine (Mac/Windows/Linux).

Now execute the following instructions in your terminal (Mac), cmd (Windows), or Debian/Ubuntu (Linux)

```conda info --envs```

Running this command you should see one environment listed ```base```. We are going to create a clone of the base environment called ```ml``` which should have everything we need installed.

```conda create --name ml --clone base```

Now run ```conda info --envs``` again and you should see the environment ```ml``` listed. When we are coding we always want to have our ```ml``` virtual environment active rather than our ```base``` environment because we are going to install things to the ```ml``` environment and keep them separate. To activate the ```ml``` environment run the following:

```conda activate ml```

You should see the ```ml``` environmengt is now active. You can run the python command line interpreter by executing the following line:

```python```

Now the python command line interpreter is active try running a few simple commands like ```1+1```, ```1>2``` and ```100/5```. To exit the python interpreter execute ```exit()```. We will do the majority of our coding in jupyter notebooks but sometimes its helpful to run a few things in the command line when you are debugging your code. First let's create a new working directory:

```mkdir new_dir```

Then let's navigate to this new directory:

```cd new_dir```

Let's list everything in the new directory (Mac/Linux):

```ls```

Or for Windows:

```dir```

The directory should be empty because we just created it. Now let's open jupyter notebook in this directory simply run:

```jupyter notebook```

Your brower should then open and you can create a new notebook and start coding in python!

## Setting up PyTorch

We won't need this for the first half of the course but you are welcome to set this up in advance or when we start using neural networks. Open your terminal/cmd/Debian/Ubuntu and activate your conda environment:

```conda activate ml```

Now go to the [PyTorch](https://pytorch.org/get-started/locally/) website and execute the corresponding command in your terminal. The command may change whether you have a Mac, Windows or Linux. And whether you have a CUDA enabled GPU or not. Some examples, 

Mac or Windows (without GPU):

```pip3 install torch torchvision torchaudio```

or 

```pip install torch torchvision torchaudio```

Linux (without GPU):

```pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu```

Windows with GPU and latest CUDA driver (12.4+):

```pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124```

or

```pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124```

If you want to use PyTorch with CUDA enabled make sure your GPU driver is up-to-date and you know what the maximum compatibility is. Most of the time you can work this out by running:

```nvidia-smi```

And check the CUDA version.




