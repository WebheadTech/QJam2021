# QJam2021
Team Quantum Realm QJam2021 Submission

# Purpose and Goal
## Research
An overall goal was to get a working example of a QCNN.  This was our initial end goal in our research exercise.  We reviewed various papers and sample code from several websites.

## Working Example
The goal of the code was as follows:
We attempted to categorize two photos using a quantum neural network (cat and frog).
A similar investigation was conducted using the mnist data set; however, because the three-color channel was fixed in the cifar data set, we encountered some challenges and determined our accuracy value to be about 0.50. A 28x28 picture is far too huge for today's quantum computers. Resize the picture to 4x4 and 3x3 pixels. We achieve better results with 4X4, but we plan to use Quantum Image Processing - FRQI and NEQR Image Representations in the future because it's more accurate.

# Environment
Our team tried various environments/frameworks like Anaconda and Google Colab.  After several trials we decided to go with Google Colab since Tensorflow was developed by Google.
We considered other tools like PennyLane and IBM Q Experience, but we didn't have time to run against those systems however we can attempt to in the future.

## Packages
We utilized a library for some of the data preparation steps which is in folder eecs598.  You must upload this folder to your enviornment and reference.  We mounted our Google Drive and then reference the folder.

In order to run the code you may need to install/re-install/uninstall various packages.  We left these install lines in the code in case a user needs to use them.
* You may need to uninstall TensorFlow if it is not 2.5.1.  (This code may work with TensorFlow 2.4.1 as well.)
We uninstalled Tensorflow 2.7.0 and installed 2.5.1.
* We also had to install the nightly update, tfq-nightly, after installing Tensorflow Quantum.
* Import tensorflow.keras vs. keras as the versions may be different.  We installed keras 2.6.0 but after some problems we resorted to using tensorflow.kers vs. keras.
* tensorflow-estimator==2.5.* - this may not have been necessary, but we installed it anyway per some article on Stack Overflow

## Restarts
During installation you may need to restart your kernel and that might also cause you some problems.  You may need to re-run all prior cells.  Also, when re-loading notebooks the next day, we sometimes had to reload packages.

# Execution
The code will run all the way through, but the model fit step will take 45 minutes per epoch and we ran for 3 epochs.
