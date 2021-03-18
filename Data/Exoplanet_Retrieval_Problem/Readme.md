# Transmission spectra of exoplanets


The dataset is divided into a training and test set (Training: training.npy; Test: testing.npy).

The files contain Nx18 arrays, where the first 13 columns are the transit depths (in percentages) and the other 5 the corresponding parameters.

The parameters are: temperature, log(H2O), log(HCN), log(NH3) and a grey cloud opacity.

There is also an actual observation of WASP-12b, which you can use to test your trained machine learning algorithm.

The training and testing datasets don't contain the wavelength values, but these can be taken from the WASP-12b observation.
