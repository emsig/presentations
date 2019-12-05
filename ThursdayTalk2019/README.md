# Thursday Talk 5th December 2019

(TU Delft; Faculty of Civil Engineering and Geosciences > Department of
Geoscience & Engineering > Section of Applied Geophysics \& Petrophysics)

## Title

3D CSEM modelling in the frequency and Laplace domains

## Abstract

Three-dimensional controlled-source electromagnetic responses are
generally calculated directly in the domain you want to process or invert
the acquired data, hence either in the frequency or in the time domain.
However, it has been shown that modelling time-domain data with a
frequency-domain code can be competitive if a sufficiently powerful
solver is available and with appropriate frequency selection and
interpolation. I was able to speed-up the calculation of time-domain data
with a frequency-domain code by a factor of 10, speak minutes instead of
hours. The main reasons for the significant speed-up are (a) using an
adaptive gridding scheme with a flexible number of cells in each
direction and (b) using a Fourier transform with logarithmic spacing and
which requires only the imaginary part of the frequency-domain response.
An idea to further speed-up the calculation is to carry out the
calculation in the real-valued Laplace domain instead of the
complex-valued frequency domain. Initial tests to design a DLF for
Laplace-to-time transformation and applying it to semi-analytical layered
model responses were successful and very encouraging. However, applying
it to 3D responses with less precision revealed a weakness of the
Laplace-to-time transform, which I could then demonstrate with analytical
data too. I will also present the European Research project I work for,
and emg3d, our new, recently open-sourced 3D CSEM modeller in Python.
