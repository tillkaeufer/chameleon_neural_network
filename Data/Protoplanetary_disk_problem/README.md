# Protoplanetary disk data

This dataset can be used to emulate the SED modelling process of a protoplanetary disk.

The data set is divided into a training and test set (Training: X_train, y_train ; Test: X_test y_test).
All data that is marked as X should be the input of your algorithm, which predicts y.
X consists of 11 different parameters that are used to describe a model setup.

They are (Parameter: Number):'Teff[K]':0, 'Lstar[Lsun]':1, 'fUV':2, 'Mdust[Msun]':3, 'inclination':4, 'Rin[AU]':5, 'Rout[AU]':6, 'epsilon':7, 'beta':8, 'settle':9, 'amin[mic]':10

For some of them a logarithmic scale was applied (Parameter [0,1,2,3,5]).
There are more parameters that describe a model in general, but these are the parameters that vary within the data.  

![Here you can see how X_train[0] looks like.](../../images/input_0.png) 

MCFOST was run with these parameters as input and produced SEDs as output.
The y arrays have all SED data. One SED consists of 57 flux measurements at different wavelength.  

![Here you can see how y_train[0] looks like.](../../images/output_0.png) 

The wavelength for every SED point are given in position.npy. This is not needed for the training, but maybe later during the analysis.

