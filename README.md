# Instrument Classifier
The aim of this project is to classify which instrument is playing in a piece of classical music. Read more about it in A9_report.pdf.

## Code
The code is split into four parts:
* Exploration. Here we explore the data, see how many samples we can use, what is the distribution of instruments, etc.
* Database creation. Here we process raw data from [IRMAS](https://www.upf.edu/web/mtg/irmas) and create a CSV for the models to train on.
* Simple models. Here we use simpel AI models such as Random Forest, K-NN and Linear Regression.
* Neural network. Here we use CNN to classify the musical instrument.

The features for simple models and neural networks are different, which can be seen in the Database notebook. Data processing is done for each model individually, just before the training (in the same notebook).

## How to use it
Firstly, [IRMAS](https://www.upf.edu/web/mtg/irmas) training data has to be downloaded. Take a path to it. In the Exploration notebook, set the path to the [IRMAS](https://www.upf.edu/web/mtg/irmas) and run all the blocks.

#### Requirements
The feature extraction uses the following libraries: 
* [pyMIR](https://github.com/jsawruk/pymir)
* [pyACA](https://pypi.org/project/pyACA/)
* [timbral models](https://github.com/AudioCommons/timbral_models)
* [Sound File](https://pypi.org/project/SoundFile/)
* [pyloudnorm](https://pypi.org/project/pyloudnorm/)

AI models use:
* [scikit-learn](https://sklearn.org/)
* [pandas](https://pandas.pydata.org/)
* [TensorFlow](https://www.tensorflow.org/)
* [Keras](https://keras.io/)

Other requirements:
* [matplotlib](https://matplotlib.org/)
* [seaborn](http://seaborn.pydata.org/)

If there are some missing, look for them from [IDS](https://courses.cs.ut.ee/2020/ids/fall).

#### Simple models
To use simpel models on the data, open the Database notebook and run until before 'For NN' chapter. Make sure that you set the path in the first code block to the [IRMAS](https://www.upf.edu/web/mtg/irmas) root folder. Wait for the file to be created. Then open the SimpleModels notebook and run all the blocks!

#### Neural network
Set the correct path in Database notebook as in previous chapter. The run the notebook first code block and starting from 'For NN' chapter. Wait for the file to be created. Then open CNN notebook and run all the blocks!
