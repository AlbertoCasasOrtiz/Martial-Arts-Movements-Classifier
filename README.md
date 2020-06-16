# Martial Arts Movements Classifier

This Google Colab Notebook has been created for create classifiers of martial arts' movements.

## Dataset

The dataset has been captured using the sensors of an android device. It consist in a collection of CSV files, each one containing a set of columns defining the different sequences measures (Acceleration, rotation, magnetic field...).

This notebook should work with any dataset consisting in CSV files containing data organized in columns.

## Neural Networks

Three different types of neural networks have been used in this notebook for training three models:
* **FC-ANN**: A Regular fully connected neural network.
* **1D-CNN**: A 1D Convolutional neural network.
* **LSTM**: A Long short-term memory neural network.

Right now, the models only have one layer per each one of these neural networks because it gave good results. It can easily be extended for using more layers.

## Usage

Put the CSV files inside a folder named "movements", selecto some values for the hyperparameters and execute all cells in the notebook. If no errors occur, the following files are generated:

* **model.json**: Description of the model in JSON format.
* **model.h5**: Weights of the model in H5DF.
* **model_full.h5**: Description of the model and weights in a single H5DF file.
* **model.tflite**: Description of the model and weights in tensorflow lite format. This is the file used when loading the model on an Android app.
* **history.csv**: Temporal evolution of accuracy and loss for the training set and the test set in CSV format.
* **history.json**: Temporal evolution of accuracy and loss for the training set and the test set in JSONformat.
* **accuracy.png**: Chart with the temporal evolution of accuracy during training.
* **loss.png**: Chart with the temporal evolution of loss during training.
* **results.txt**: File containing final accuracies over training and testing sets, and the execution time.
* **model_plot.png**: Graphical description of the model.


## License
This software is licensed under the [AGPL](https://choosealicense.com/licenses/agpl-3.0/) license.
