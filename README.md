Prokcounter_imageJ
==============
Version v0.1-10112011
Giovannelli & d’Errico 2011
This work is licensed under a Creative Commons Attribution 4.0 International License
http://creativecommons.org/licenses/by/4.0/


This macro counts and measures the area of prokaryotes (or any other cells or particles present in the picture) using the particle analyzer and splitting image channels according the fluorescence recorded. 

In this case the macro is set to work with the green fluorescence of Acridine Orange used to count prokaryotes in sediments or water by mean of epifluorescence microscopy (see Hobbie, J.E., Daley, R.J. & Jasper, S. 1977. Use of nuclepore filters for counting bacteria by fluorescence microscopy. Appl. Environ. Microbiol. 33, 1225–1228 for additional details). 

Dimension, circularity and threshold level are sample/tissue/cells specific and should be evaluated accordingly in a preliminary phase before to set up the macro parameters. At the end of the measurement save the summary windows containing the results.

//Installation//

- Download and install ImageJ or Fiji according to the guideline on the respective sites. Google ImageJ or Fiji image analysis software if you need to

- Download the Prokcounter script and copy it in the imageJ/macros folder or subforlder

- Start imageJ (or Fiji). You can now run the Prokcount macro using the Plugins>Macro>Run... menu

//Use and calibration//
Before making automatic measurement of the cells/particle, you should calibrate the script. 

CALIBRATION: Use an appropriate number of micrographs (>10) to manually measure the minimum and maximum dimension of the particles you are interested in, and their circularity. Calculate an average min and max dimension and the average circularity for your sample. Edit the prokcounter_imagej.java file using a text editing file (such as Gedit) and change in line 31 the min-max size and the min-max circularity. Sometimes also the threshold value (line 25) has to be changed depending on the amount of background fluorescence present in your sample. This can be determined manually using Threshold option in the manu image>adjust>threshold.

DATA ACQUISITION: Save all image from the same sample in a folder. use different folder for different samples. Run the prokcount macro for every folder and record the results.

