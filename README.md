# Global-Structural-Earthquake-Damage-Prediction
Using deep learning techniques to detect damage in a structure(G+20 building) with hinges formation in joints after an earthquake.
The networks used to train the data includes: '1D Convolutional Neural Network', 'LSTM Network', '2D Convolutional Neural Network using spectrograms'.
Data is recorded for X & Y axes using accelerometers attached to the joints of the structure and the cases of earthquakes are generated by providing impulses to the structure using SAP2000.

Data for training can be found at (Please refer to the .zip file of the dataset):

https://drive.google.com/file/d/1zBAMNiHTHqJS5fIZSiklUlsfCli9HM82/view?usp=sharing

For data used in the Predictions notebook, refer to:

https://drive.google.com/drive/folders/1Gzo2Zqh0XB43IqyGRfU_rCcj8ABOBTeY?usp=sharing

Once you check the data, file 'Data and Discrepancies.txt' describes the discrepancy found in each of the cases in data.

* Refer to file 'Earthquake Damage Detection-2 Data Preprocessing.ipynb' for processing the data.

* Refer to the file 'Earthquake Damage Prediction-2 Preparing I&O.ipynb' for preparing the data to be fed into networks and generating the spectrograms for both X&Y axes.

* Refer to the file 'Earthquake Network Training 3.ipynb' for training 1D CNN and LSTM. The attached notebook might contain the code for training the 2D CNN using spectrograms as   well but the training is done in a seperate notebook.

* Refer to the file 'Earthquake Network Training 2 Layered 1D CNN & Spectrogram Training.ipynb' for training a 2 Layered 1D CNN (as a part of multiple experimentations performed     using 2, 3, 4 layers of 1D CNNs) and the 2D CNNs using spectrograms.

* Refer to the notebook 'Copy of SHM_Notebook.ipynb' for Grid Searching the optimized hyperparameters in 1-D CNN and LSTM (since both outperformed the conventional 2-D CNN and       would later be ensembled in future developments to improve the predictions).

* Refer to the notebook 'Predictions.ipynb' to refer to the predictions provided by the trained networks on an untouched data.
