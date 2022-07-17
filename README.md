# Final project of Image Processing and Analysis course

Student: R.R.M.  
nº USP: 6516211

**Warning!**
The images in this repository may be disgusting to some people.

## Project proposal theme in a sentence
Segmentation and analysis applied to photos of bird droppings for morphological characterization

##  Abstract
Excrements (also called bird droppings) of a healthy bird consists of two phases: a long cylindrical green solid shape immerse in a heterogeneous white and translucid liquid.
This morphology is subjected to some expected variance due to random bird alimentary routines, like the quantity of water and the type of food ingested.
However, health conditions and sensibility to some kind of food may significantly disturb the usual morphology and color of the excrements, for example when occur diarrhea or bleeding.

In this project, a set of photos of healthy _psittacidae_ morning droppings was processed to extract descriptors reflecting the usual morphology characteristics.
These descriptors comprehended: area measurement, texture information and color information.
All measurements from these healthy droppings were gathered to compose normality curves on each descriptor, which may be useful for the detection of future anomalous droppings that might significantly deviate from the expected values.

Photos have been taken personally by the student using a DSLR camera with the dropping placed on a clean sheet of white paper along a brown reference scale of constant and known size.

Segmentation and feature extraction were the main processing tasks done.
Segmentation was done using limiar thresholds with python slicing on Saturation and Luminance.
Feature extraction was done using Fourier transformation, Histogram calculation and Haralick descriptors.

The normality curves/histograms were generated, but, unfortunately, the detection of anomaly was unsuccessful.
However, there are several opportunities for improvement.

Further details on `presentation-notebook.ipynb`
