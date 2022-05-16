Algorithm and data for seismic traveltime inversion tomography beneath the Malay Peninsula

1. Unzip the "Algorithm_&_files" folder

Inside the folder are:
a) "output_files_15m" folder (contains output files of the 0.25º grid spacing)

b) "output_files_30m" folder (contains output files of the 0.5º grid spacing)

c) "gmt_codes" folder (contains gmt codes to produce the figures)

d) some other files (i)-(vi):
i)   DATA_PRE (arrival time dataset)
ii)  A_PARAM_MALAY.INC (contains all parameter settings)
iii) STN_GLOBAL (Station list)
iv)  VEL_MODELS (different 1D Velocity Models)
v)   VELMODE.exe (the executable file)
vi)  VELMODE.for (the Fortran code)

2. Run the VELMODE.exe file by double clicking
   Enter "1" to use the default settings
   After a few seconds, the output files will be generated
   
3. To run a checkerboard resolution test
a) Enter "2"
b) Enter "2" to select the ak135 velocity model
c) Enter "1" to use p wave for inversion
d) Enter "1" to perform perturbation
e) Enter 2 for a 2% perturbation
f) Enter 1 for a simple alternating grid separation  
After a few seconds, the checkerboard output files will be generated

(Note that the 0.25º grid spacing is the default. You can change to the 0.5º grid spacing in the A_PARAM_MALAY.INC file)
   
4. Open the "gmt_codes" folder to find several ".bat" files (gmt codes to generate figures from several output files)
(a) copy all the .bat files into the "Algorithm_&_files" folder
(b) files with *_15m.bat files are for the  0.25º grid spacing output
(c) files with *_30m.bat files are for the  0.5º grid spacing output
(d) run the various *_15m.bat files to create the figures for the  0.25º grid spacing output
(e) run the various *_30m.bat files to create the figures for the  0.5º grid spacing output

Comments are provided within the algorithm
