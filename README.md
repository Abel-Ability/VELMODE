# VELMODE
Algorithm and data for seismic traveltime inversion tomography beneath the Malay Peninsula

1. Unzip the folder "Algorithm_and_files" to see 7 files
(i)   A_DATA_PRE
(ii)  A_PARAM_MALAY.INC
(iii) STN_GLOBAL
(iv)  VEL_MODELS
(v)   VELMODE.exe
(vi)  VELMODE.for
(vii) VELMODE.txt

Input files:
 (a) STN_GLOBAL (Station list)
 (b) VEL_MODELS (different 1D Velocity Models) 
 (c) A_DATA_PRE (arrival time dataset)

2. Run the VELMODE.exe file. Use default settings by entering the option "1"

3. To run a checkerboard resolution test:
  (a) Enter "2"
  (b) Enter "2" again at the next prompt to select the ak135 velocity model
  (c) Enter "1" to use p wave for inversion
  (d) Enter "1" to perform perturbation
  (e) Enter 2 for a 2% perturbation z
  (f) Enter 1 for a simple alternating grid separation
  (g) Enter "0" to skip relocation of events
  
4. Comments wihin the subroutines explains their functions

Output files:
    A10_EVENTS.TXT             (EVENTS USED)
    A11_SUMMARY.TXT            (SUMMARY OF COMPUTATION)
    A12_RESIDUALS.TXT          (TRVEL TIME RESIDUALS)
    A13_MODEL_3D.TXT           (MODEL-3D)
    A14_SLICE_DEP.TXT          (MODEL-DEP SLICES)
    A15_SLICE_LAT.TXT          (MODEL-LAT SLICES)
    A16_SLICE_LON.TXT          (MODEL-LON SLICES)
    A17_RAYPATH_D.TXT          (DIRECT WAVE ARRIVAL (OPEN IF REQUIRED))
    A18_RAYPATH_R.TXT          (REFRACTED WAVE ARRIVAL (OPEN IF REQUIRED))
    A19_RAYPATH_D_ALL.TXT      (ALL BDR DIRECT RAYS (OPEN IF REQUIRED))
    A20_RAYPATH_R_ALL.TXT      (ALL BDR REFRACTED RAYS (OPEN IF REQUIRED))     
    A21_CKB.TXT                (CKB MODEL (OPEN IF REQUIRED))
    A22_PTB-PRIORI             (TO OBSERVE ANY CHANGE IN SIGN WHEN CKB IS INVERTED)
    A23_NEWHYPO.TXT            (RELOCATED EVENTS (OPEN IF REQUIRED))
    A31_AVE_RES.TXT            (AVERAGE RESIDUALS (ALL AZIMUTH) (OPEN IF REQUIRED))
    A32_090.TXT                (AVERAGE RESIDUALS (0=AZIMUTH<090) (OPEN IF REQUIRED))
    A33_180.TXT                (AVERAGE RESIDUALS (90=AZIMUTH<180) (OPEN IF REQUIRED))
    A34_270.TXT                (AVERAGE RESIDUALS (180=AZIMUTH<270) (OPEN IF REQUIRED))
    A35_360.TXT                (AVERAGE RESIDUALS (270=AZIMUTH<360) (OPEN IF REQUIRED))
    A36_STN_USED.TXT           (LIST STATIONS USED (FOR GMT STATION PLOT))
    A_DATA_PRE                 (EVENTS AND STATION ARRIVAL TIMES (FROM (ISC, JWEED, SFILE, ETC))
    A_DATA1                    (DATASET BEFORE RELOCATION)
    A_DATA2                    (DATASET AFTER RELOCATION)
    

