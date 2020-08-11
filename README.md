# lyapunov-hyperopt
The lyapunov.py module contains the code used to calculate Jacobians and lyapunov exponents. The code is written primarily using Pytorch

The primary methods to look at in that module are calc_LEs_an and LE_stats. The first calculates the exponents for given network with a batch of inputs. These results can be passed to LE_stats in order to find the mean and standard deviation of the exponents over that batch.


Sample calculations can be found in the CharRNN notebook. Configuration classes, found in config.py, are used for the loading of data, model, and training. The parameters of these configurations determine the name of the experiment in the FullConfig. A separate configuration object is used for the calculation of the Lyapunov Spectra.
