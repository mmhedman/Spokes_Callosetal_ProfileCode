# Spokes_Callosetal_ProfileCode
Code and output for Generate profiles of Spoke activity from Callos et al. 2025 (PSJ 6:17)

Includes the Jupyter Notebook Spokiness_Processing_Code_public.ipynb, which contains a program that reads a set of IDL save files containing maps of the B ring (not included, can be reconstructed from fits files and their labels stored on the PDS), which is then run on multiple sets of images to produce profiles of the spoke activity and the background ring brightness that are plotted in Figures 10-12 of the paper. This code includes the explicit parameters for each observation.

It also contains sub-directories of the outputs from the program, the directory Profiles contains files containing the profiles of s(r) and I/Fb for each individual image, while signals and backgrounds contains files giving the average profiles for each observation.
