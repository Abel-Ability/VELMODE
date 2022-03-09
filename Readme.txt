Algorithm and data for seismic traveltime inversion tomography beneath the Malay Peninsula

1. Unzip the folder "Algorithm_and_files" 

Inside the folder are the files:
a) A_DATA_PRE (arrival time dataset)
b) A_PARAM_MALAY.INC
c) GMT_Figures.bat (GMT code to generate figures of the inversion results) 
d) GMT_Figures_CKB.bat (GMT code to generate figures from the checkerboard test)
e) STN_GLOBAL (Station list)
f) VEL_MODELS (different 1D Velocity Models)
g) VELMODE.exe (the executable file)
h) VELMODE.for (the Fortran code)
i) VELMODE.o

2. Run the VELMODE.exe file. 
   Enter "1" to use default settings
   
3. Doubleclick the file "GMT_Figures.bat" to run the output files
A14_SLICE_DEP.TXT, A15_SLICE_LAT.TXT and A16_SLICE_LON.TXT

4. To run a checkerboard resolution test
a) Enter "2"
b) Enter "2" to select the ak135 velocity model
c) Enter "1" to use p wave for inversion
d) Enter "1" to perform perturbation
e) Enter 2 for a 2% perturbation
f) Enter 1 for a simple alternating grid separation

5. Doubleclick the file "GMT_Figures_CKB.bat" to run the output files
A14_CKB_DEP.TXT, A15_CKB_LAT.TXT and A16_CKB_LON.TXT

Comments have been provided within the algorithm
