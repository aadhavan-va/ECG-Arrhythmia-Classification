# ECG-Arrhythmia-Classification
ECG arrhythmia classification using Convolutional Neural Network

![ecg-ml](https://user-images.githubusercontent.com/51418721/89326068-5b6d6580-d6a7-11ea-8d43-7d8a77855200.gif)
<br>
## Dependencies
**1. wfdb**<br>
**2. biosppy**<br>
**3. py-ecg-detectors**<br>
**4. Tensorflow**<br>
**5. Keras**<br>

## Working
The model helps in diagonising the irregular heart rhythms,also known as arrhythmias,from the ECG samples of the patients.The dataset for performing classification was taken from the MIT-BIH database(https://physionet.org/) contains 48 half-hour of two-channel ambulatory ECG recordings.<br>
The ECG annotated files are first converted into images using Wfdb provided by the MIT-BIH database and biosppy library for detecting the rpeaks of the annotated ECG signals.The rpeaks were first take from the signals and the using various annotations available in the MIT-BIH description page the Arrhythmia images are generated.In order to obtain high accuracy the images are augmented using ImageGenerator function available in tensorflow library.
The 2D ECG images are then passed into the neural network architecture and the accuracy of the model are obtained.<br>
The ECG images are then tested with the pre-trained CNN architecture provided by the keras InceptionV3 and the model preformed well with the ECG images.<br>
[Dataset for ECG Arrhythmia detection](https://physionet.org/content/mitdb/1.0.0/)
