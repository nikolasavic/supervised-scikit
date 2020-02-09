Running the code:
=================
1) Install Anaconda following instructions here: https://docs.anaconda.com/anaconda/install/

2) Start Jupyter Notebook server with the following command: `jupyter notebook`

3) You can run all cells to get the complete report, although it may take some time. Or if
   you just want the final fit, the training results and the test results, run all the cells
   below the markdown cell labeled "Fit".


Versions:
=========
Scikit Learn:     0.22
Numpy:            1.17.4
Pandas:           0.25.3
Matplotlib:       3.1.1
Python:           3.7.5
Juypter Notebook: 6.0.2


Data:
=====
There is no need to manually download the data since the code takes care of that for you, but if
you're interested it can be found here:
  MNIST: https://www.openml.org/d/554
  Credit: https://www.openml.org/d/31


Performance:
============
Running all of the cells may take a very long time (days), in addition there are many cells that take advantage
advantage of multithreading and use the `n_jobs=-1` parameter to use all available cores.  The SVM notebook uses
a larger cache_size, to increase speed.

Don't forget to adjust these values to match your system if running these cells.


Notes:
======
 - There are five files, each dedicated to a single algorithm and both data sets as well as 
   one file used for data exploration purposes.

 - All the algorithm files are structured in a similar way, and use the same random state seed.
   The test/train split occurs before the data is standardized to avoid fitting on the test set.
