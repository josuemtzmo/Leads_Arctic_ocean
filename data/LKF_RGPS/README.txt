LKF data-set (winter 1996/1997 to 2007/2008)

Linear Kinematic Featuress (leads & pressure ridges) detected and tracked in RGPS deformation data, that is described in Hutter et al. (2019).

Data-Sources:
- Deformation: RGPS Eulerian gridded deformation data (https://rkwok.jpl.nasa.gov/radarsat/index.html)
- Drift: RGPS Lagrangian Drift product (https://rkwok.jpl.nasa.gov/radarsat/index.html)



Data Description:

The data set covers all RGPS winter data, i.e. November to May for the years 1996/97 to 2007/08. The LKFs of each winter season are saved in one TAB-delimited text-file (ASCII). In total the data-set contains in 12 files.

In the csv-file each row corresponds to one pixel of an LKF in this year. In individual pixels are sorted by date and LKF. Each LKF gets a identifier number (LKF No.) that is unique in this winter. For track features the LKF No.(s) of parent LKF(s) from the previous RGPS time record are provided.  

The columns of the csv-files are structured in the following way:
Start Year, Start Month, Start Day, End Year, End Month, End Day, Date(RGPS format), LKF No., Parent LKF No., lon, lat, ind_x, ind_y, divergence rate, shear rate

Specific comments:
Start Year, Start Month, Start Day -> Start date of the RGPS time record in which LKFs are detected
End Year, End Month, End Day       -> End date of the RGPS time record in which LKFs are detected
Date in original RGPS format       -> RGPS format of date (first for digits are the year, the last three digits are the number of days). This format is used as filename by RGPS.
LKF No.                            -> each LKF in one winter has its unique identifier number that can be used to track the feature
Parent LKF No.                     -> LKF No. of the LKF from the previous time records, for that this LKF is a temporal continuation determined by the tracking algorithm. This entry can contain multiple numbers if the current LKF was formed from multiple LKFs. '0' is used as a fill value, if there is no parent LKF.
lon, lat                           -> position of LKF pixel
ind_x,ind_y                        -> Indexes of the LKF pixel in original RGPS data that can be used to index original RGPS fields
divergence and shear rate          -> The divergence and shear rate of RGPS deformation data at LKF pixel. The divergence rate can be used to distinguish leads and pressure ridges in the data-set, please see Hutter et al. (2019).


Literature:
Hutter, N., Zampieri, L., and Losch, M.: Leads and ridges in Arctic sea ice from RGPS data and a new tracking algorithm, The Cryosphere Discuss., https://doi.org/10.5194/tc-2018-207, in review, 2018.

This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.
