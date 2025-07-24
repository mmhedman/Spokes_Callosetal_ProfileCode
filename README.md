# Spokes_Callosetal_ProfileCode
Code and output for Generate profiles of spoke activity from Callos et al. 2025 (PSJ 6:17, DOI: 10.3847/PSJ/ad9583))

Includes the Jupyter Notebook Spokiness_Processing_Code_public.ipynb, which contains a program that reads a set of IDL save files containing maps of the B ring (not included, can be reconstructed from FITS files and their labels stored on the PDS, available via https://pds-rings.seti.org/pds4/bundles/cassini_iss_spokes_hedman-hamilton-2025), which is then run on multiple sets of images to produce profiles of the spoke activity and the background ring brightness that are plotted in Figures 10-12 of the paper. This code includes the explicit parameters for each observation.

It also contains sub-directories of the outputs from the program, the directory "Profiles" contains files ending in "sigprofs.txt" and "backprofs.txt" that contain profiles of s(r) and I/F_b(r) for each individual image in a selected observation (indicated by the first part of the filename) that can be used to generate profiles like that shown in Figure 10. For each of these files the first column gives the ring radius, and the subsequent columns give the relevant parameter for each of the different profiles. The number of columns is determined by the number of images in the selcted observation. 

The directories "Signals" and "Backgrounds" contain files that provide summary profiles for each observation indicated by the start of the relevant filename, which can be used to generate the profiles shown in Figures 11 and 12. The files in "Backgrounds" each just have two columns, which are the radius and mean I/F_b values for the relevant observation. The files in "Signals" have four columns. 

The first columns gives  is the observed radius.
The second column is the difference between the average and minimum value of the spoke signal s at that radius, which can be used to compute the \bar{n}' parameter.
The third column is the difference between the maximum and minimum value of the spoke signal s at that radius, which was not used in the paper.
The fourth column is the average value of the spoke signal s at that radius, which can be used to compute the \bar{n} parameter. 
