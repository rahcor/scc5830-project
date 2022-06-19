# Final project of Image Processing and Analysis course

Student: R.R.M.

**Warning!**
The images in this repository may be disgusting to some people.

## Project proposal theme in a sentence
Segmentation and analysis applied to photos of bird droppings for morphological normality characterization.

##  Abstract
Excrements (also called bird droppings) of a healthy bird consists of two phases: a long cylindrical green solid shape immerse in a heterogeneous white and translucid liquid.
This morphology is subjected to some expected variance due to random bird alimentary routines, like the quantity of water and the type of food ingested.
However, health conditions and sensibility to some kind of food may significantly disturb the usual morphology and color of the excrements, for example when occur diarrhea or bleeding.

In this project, a set of photos of healthy _psittacidae_ morning droppings will be processed to extract descriptors reflecting the usual morphology characteristics.
These descriptors will comprehend: area measurement, texture information and color information.
All measurements from these healthy droppings will be gathered to compose normality curves on each descriptor, which may be useful for the detection of future anomalous droppings that might significantly deviate from the expected values.

Photos have been taken personally by the student using a DSLR camera with the dropping placed on a clean sheet of white paper along a brown reference scale of constant and known size.


## Expected steps in processing the images

* K-means is applied to the original images to segment the background, the reference scale, the solid green phase and the liquid white/translucid phase.
* From the reference scale, the ratio area/pixel will be calculated and the white balance will be adjusted to match the reference scale color.
* From the group containing solid and liquid dropping, the total area will be measured^1, homogeneity descriptor will be calculated^2, fft spectrum will be derived and the full image submitted to bag of features.
* From the solid/green segment, area, color histogram^3 and homogeneity^2 descriptor will be gathered.
* From the white segment, area and color will be measured.
* Finally, the proportion of area of solid and white^4 will be calculated.

The numbers above some words in the previous list corresponds to some health conditions that the measurement tries to capture:

^1 Small intake of food
^2 diarrhea
^3 blood
^4 imbalance in water/food intake


### Summary of methods that are expected to be employed

* Segmentation using K-means
* Counting pixels
* Haralick descriptors
* Color histograms
* FFT spectrum
* Bag of features


## Output expectation 

Three types of normality curve are expected as output:

* absolute value (area, Haralick)
* distribution of distances between images (histogram, fft spectrum)
* distribution of distances from the mean (features from bag of features)
