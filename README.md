# **CONVOLUTION REVERB**

Convolution reverb is an exciting technique of bringing new space into the sounds. The
program built in Python 3 digitally simulates the reverberation of a physical or virtual acoustic
space with the help of a program. It convolves an input signal with the impulse response of an
actual or a virtual acoustic space creating an illusion as if the input signal was recorded in that
acoustic space. The output audio signal reflects the sonic qualities of the selected acoustic
environment. This technique is widely used in Electronic Music, Machine Simulation and Real
Space Simulations.

## **Libraries:**

### Pre-existing libraries:
-> scipy.io

-> numpy

-> matplotlib.pyplot

-> sounddevice

-> time

-> sys

### Need to pip install:
-> tqdm

-> ipython

>from tqdm import tqdm_notebook as tqdm

>from IPython.display import Audio

## **Description:**
The program convolves an input signal with the impulse response of an actual or a virtual
acoustic space creating an illusion as if the input signal was recorded in that acoustic space.
Impulse response is a short and a sharp sound like the sound of a gunshot, church bell and
popping of a balloon etc. The impulse response recording should contain the widest range of
frequencies in the reverb reflections as far as possible. The program entreats the user to choose
a music file (or the user can lively record audio) and asks the user to select an environment.
The sampling rate for all the signals used is set at a default sampling rate of 44100 Hz.
The chosen audio file is then convolved with the pre-recorded impulse response of the
selected acoustic environment producing an output audio signal which reflects the sonic
qualities of the selected acoustic environment. To speed up the process of convolution both the
input signal and the impulse response of the acoustic environment are transformed from time
domain to frequency domain using Fast Fourier Transform (FFT) and then multiplied (as
convolution in time domain is multiplication in frequency domain).
The final signal is then inverse transformed using Inverse Fast Fourier Transform (IFFT).
Then the output time domain signal is sampled at the default sampling rate and the program
asks the user to input a panning (Panning is the spread of a monaural signal in a stereo or multi-
channel sound field) rotation count. The final signal is panned left and right gradually the as
per the number of times the user entry in panning rotation count. Finally, the signal is converted
into an uncompressed universal audio file format (.wav). If required the user can download the
final audio file in .wav file format.

## **IDE Used:** Python 3.8 Anaconda Distribution → Jupyter Notebook
## This program is designed to run in **NOTEBOOK IDE**
