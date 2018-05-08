


# Car Evaluation using PyTorch Neural Network

Here is my attempt of building a Neural Network classifier using PyTorch.

### Dataset

This datset is available [here](http://archive.ics.uci.edu/ml/datasets/Car+Evaluation). It is derived from simple hierarchical decision model, this database may be useful for testing constructive induction and structure discovery methods.

### Attribute Information

The dataset consists of a class label with 4 different values : unacc, acc, good, vgood.

There are 6 attributes as follows:

- buying: vhigh, high, med, low. 
- maint: vhigh, high, med, low. 
- doors: 2, 3, 4, 5more. 
- persons: 2, 4, more. 
- lug_boot: small, med, big. 
- safety: low, med, high. 


### Getting Started
  - The code is written in python.
  - I have used Jupyter notebook for easier understanding and execution of the codes.
  - Tutorial on how to use [Jupyter](https://jupyter.readthedocs.io/en/latest/) notebook.

If any libraries are missing on the system simply pip install them and re-run the code
```
pip install <module>
```

### Project Files

*	[Dataset](https://github.com/ritvikkhanna09/Car-evaluation-ml/tree/master/Datasets)
*	[PyTorch Script](https://github.com/ritvikkhanna09/Car-evaluation-ml/blob/master/Script.ipynb)
*	[Visualization of Dataset](https://github.com/ritvikkhanna09/Car-evaluation-ml/blob/master/Visualisation.ipynb)


### Results

Here, the dataset contains of 6 attributes and 1 class column having 4 class values{unacc, acc, good, vgood}. As we are building a neural network we need to provide the each neural node values it can read and not be bias over a specific value of an attribute.

Earlier, I used simple method the dummies for each value in the attribute column was not used, the accuracy obtained was **75%**.

Therefore we convert all the nominal/categorical data into numeric by using pandas.get_dummies function. This function will create additional columns of each values corresponding to each attribute, therefore increasing the number of total columns. The accuracy was better. Accuracy - **86.54%**


## Author

Ritvik Khanna

[contact](mailto:ritvikkhanna09@gmail.com)
