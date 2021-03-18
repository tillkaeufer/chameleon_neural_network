# CHAMELEON Hands-on Session Neural Networks
This Repository gives all data and information that are needed to participate in the neural networks hands-on session of the first CHAMELEON school.

# Things to install before the session

Please install the following things before the session.

- Python 3
- Jupyter Notebook </br>
For doing so, the easiest way is to create an anaconda environment: </br>
https://www.anaconda.com/products/individual </br>
If you have problems, please contact us.

Also, the following packages are needed:
- SKlearn: conda install scikit-learn
- Keras/Tensorflow: conda install tensorflow
- numpy: conda install numpy
- matplotlib: conda install matplotlib
- corner: conda install -c conda-forge corner

# General Idea

We prepared two different problems, which can be solved using Machine Learning. </br>

First problem:</br>

### Extracting exoplanet parameters using spectra.</br>
The goal here is to predict atmospheric parameters of exoplanets from their transmission spectra using machine learning.
You will be provided with a dataset containing synthetic HST/WFC3 transmission spectra of exoplanets and their corresponding parameters.
The parameters defining the forward models are: isothermal temperature; H2O, HCN and NH3 mixing ratios; and a grey cloud opacity.
The spectra consist of 13 wavelength bins between 0.8 and 1.6 microns, which match those of the WASP-12b observation in Kreidberg et al., 2015.
This observational dataset is also provided to retrieve on once your machine learning algorithms have been trained.</br>

Second problem: </br>
Emulating SED modelling of protoplanetary disks. </br>
... </br>



# Steps
- Decide on  a dataset you want to anaylze.
- Set up a notebook 
- Import the needed packages
- Inport the data
- Scale your data
- Import a ML technique and adjust it
- Analyze the results
- Start playing with different settings and techniques to find the best results

# Detailed Explanation

Set up a notebook in which you want to solve your problem.

## 1: Loading your data

You find the data for your problem in the folder 'Data'. Click on the problem you want to tackle and download the data. </br>
(You can also download the whole repository to make things easier.) </br>
Load the data into your notebook. If you feel confident you can do this without further help. </br>
If you run into problems or want to check if you have done everything right, check out the load_data.ipynb. There you find a working version for loading the data.

## 2: Scaling your data

Once you loaded the data you have to scale it. </br>
In the folder 'Scaling' you find an explanation of different scaling methods and how to apply them.
Feel free to play around and vizulize how your data is changing if you apply a scaler. </br>
Again, in the folder named after your problem you find a working example of scaling the data. </br>


## 3: Applying Machine Learning

After loading and scaling your data, it is now time to apply some Machine Learning.</br>
We focus on Neural Networks in this session, but you can also run Random Forests as a comparison.</br>

### 3.1: Build/train a Neural Network

Depending on your level of confidence you can take different approaches.
- https://victorzhou.com/blog/keras-neural-network-tutorial/ </br>
  This is a general tutorial how to build Neural Networks. Try to create your own network, which can solve your choosen problem. </br>
  There are many different ways to do that, dissusing your approaches in your group or searching on the internet can help.</br>
  We would recomend to use Keras, because all packages are installed on your environment. </br>
- If you want to have a bit more support look into the folder for your problem. There you will find an example of a suitable NN for your problem

### 3.2: Optimize your network

If you have a working network you can change the different settings and have a look how your results change. Try to find the best network for your problem.

### 3.3: Optional: Build/ train a Random Forest

If your network works and you get bored, try to solve your problem using a different ML technique. </br>
We recomend Random Forest (a few hints can be found in the 'ML_techniques' folder), but you can also apply other methods. </br>
A list of methods can be found here: https://scikit-learn.org/stable/supervised_learning.html </br>

## 4: Visualization

This point is hard to seperate from all previous steps. During the whole process you probably want to see what is going on. </br>
This is espacialy important, to evaluate your results. Think of useful ways to evaluate the results and visualize them. If you need a bit of inspiration, in the folder 'Visualization' there are a few uselfool tools.


