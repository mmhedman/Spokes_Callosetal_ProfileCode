# Spokes_Callosetal_ProfileCode
Code and output for Generate profiles of spoke activity from Callos et al. 2025 (PSJ 6:17, DOI: 10.3847/PSJ/ad9583))

Includes the Jupyter Notebook Spokiness_Processing_Code_public.ipynb, which contains a program that reads a set of IDL save files containing maps of the B ring (not included, can be reconstructed from FITS files and their labels stored on the PDS, available via https://pds-rings.seti.org/pds4/bundles/cassini_iss_spokes_hedman-hamilton-2025), which is then run on multiple sets of images to produce profiles of the spoke activity and the background ring brightness that are plotted in Figures 10-12 of the paper. This code includes the explicit parameters for each observation.

It also contains sub-directories of the outputs from the program, the directory 'Profiles' contains files containing the profiles of s(r) and I/F_b for each individual image that can be used to generate profiles like that shown in Figure 10.
while the directories 'Signals' and 'Backgrounds' contain files giving the average profiles for each observation, which can be used to generate the profiles shown in Figures 11 and 12. 
