# ReconRSI
Reconstruction Program for RSI (Rosette Spectroscopic Imaging) acquired data


Linux Installation:

If files needed and Matlab Runtime are installed within a user’s home directory, no root/superuser permissions should be required. Local installation packages (which include the Matlab Runtime) are located at  https://pitt.box.com/s/sedtq105ehmve7ni8cd5ty8h7zjk5pwp 

> ./reconRSI_localInstaller.install &
and follow directions (the default installation directories require root).

Help:

> rsi_recon -help

Usage:

> rsi_recon &

OR

> rsi_recon MetabFile GreScoutFile brainoTrueFalse savePicsTrueFalse griddingWindow WaterReferenceFile &

-MetabFile is the water-supressed RSI twix file (relative path to cwd OK)

-GreScoutFile is the GRE scout aligned with RSI, twix file. If only a RSI water reference was done but no GRE scout, enter 0 here.

-brainoTrueFalse should be entered 1 for a braino phantom  and 0 otherwise

-savePicsTrueFalse: To generate pics, this should be entered 1. If no connection to the X server, enter 0 here.

-griddingWindow can be 1.5, 2, 2.5, ... or 4

-WaterReferenceFile is the water-reference RSI twix file. If this was not acquired, no entry is required here (or enter 0 here).
