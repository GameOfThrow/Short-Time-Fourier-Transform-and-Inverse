# Short-Time-Fourier-Transform-and-Inverse
Applys the short time fourier transform and inverse of STFT in Matlab
The result is also sometimes known as a Spectrogram - used in signal processing.
The concept can be found here: http://ieeexplore.ieee.org/document/1164162/
The basics can be found here: https://en.wikipedia.org/wiki/Short-time_Fourier_transform

Note that matlab functions such as `fft` and `ifft` are used in the implementation.

To call the STFT function:

[y0,f0,t0] = sg(x,nfft,Fs,WINDOW,noverlap);
`x` is the signal vector
`nfft` is the number of FFT coefficients
`Fs` is the sampling frequency
`WINDOW` uses a window function (Matlab built-in) such as: hamming(512)
`noverlap` is the number of overlap


To call the inverse STFT function:
x = invspecgram(y0,NFFT,Fs,WINDOW,NOVERLAP);
