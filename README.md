# Sloan Sky Servey
## classification of stars, Galaxies and Quasar

   "The [Sloan Digital Sky Survey](https://www.kaggle.com/lucidlenn/sloan-digital-sky-survey/) has created the most detailed three-dimensional maps of the Universe ever made, with deep multi-color images of one third of the sky, and spectra for more than three million astronomical objects"

   "The data consists of 10,000 observations of space taken by the SDSS. Every observation is described by 17 feature columns and 1 class column which identifies it to be either a star, galaxy or quasar."

   The Analysis below, tries to study the different features of star, galaxy and quasar and uses K- Nearest Neighbours(KNN) algorithm to predict the three classes STAR, GALAXY OR QUASAR.
	

## Install

This project requires python 3.6 or anyother higher versions of python, along with these libraries

  * NumPy
  * Pandas
  * matplotlib
  * scikit-learn
  * seaborn

You also need a software to run this python notebook "Jupyter Notebook". It is highly recommended that you install the Anaconda distribution of Python, which already has the above packages and more included.



## Feature Description
The table results from a query which joins two tables (actuaclly views): "PhotoObj" which contains photometric data and "SpecObj" which contains spectral data.

   * **objid** - Object Identifier
   * **ra** - J2000 Right Ascension (r-band)-
   * **dec** - J2000 Declination (r-band)
   * **u(ultraviolet)** -  better of DeV/Exp magnitude fit
   * **g(green)** - better of DeV/Exp magnitude fit
   * **r(red)** - better of DeV/Exp magnitude fit
   * **i(Near infrared)** -  better of DeV/Exp magnitude fit
   * **z(Infrared)** -  better of DeV/Exp magnitude fit
   * **run** - Run Number
   * **rerun** - Rerun Number
   * **camcol** - Camera column
   * **field** - Field number
   * **specobjid** -  Object Identifier
   * **redshift** - Final Redshift
   * **plate** - plate number
   * **mjd** - Modified Julian Date, used to indicate the date that a given piece of SDSS data (image or spectrum) was taken.
   * **fiberid** - fiber ID

## Desired Target

  * **Class** - galaxy, star or quasar object
### Further information on SDSS images and their attributes:
(http://www.sdss3.org/dr9/imaging/imaging_basics.php)


(http://www.sdss3.org/dr8/glossary.php)


## Models Trained On

 |Algorithm       |Acuracy  |
 |----------------|--------:|                 
 |	KNN(hardcode) |   97.6% |
 |	KNN(Sklearn)  |  98.4%  |