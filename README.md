# Shear Stress Partitioning
Data for estimating friction velocity and drag partition.

## Authors
* Nancy P. Ziegler (ERDC)
* Sandra L. LeGrand (ERDC)
* Nicholas P. Webb (USDA/NMSU) 
* Adrian Chappell (U. Cardiff)

## Created 
Winter 2018/2019

## Purpose
This repository includes *in situ* and derived datasets used by Ziegler et al. for the manuscript "Insights to shear stress partitioning from land surface albedo" under consideration for pubication in JGR-Atmospheres.

## Data
Field data used for this experiment were collected from two study sites at the US Department of Agriculture - Agricultural Research Service (USDA-ARS) Jornada Experimental Range (JER) in southern New Mexico, USA (Webb et al., 2016a) and ten National Wind Erosion Research Network sites (Webb  et  al., 2016b). Data for the WEN sites can be downloaded from the public WEN data portal winderosionnetwork.org/data-portal/public-data.

*In situ* and derived data values for JER Site 3 (Playa) and JER Site 4 (Open shrubland) for the period 1 April 2018 to 31 September 2018 are included in this repository.  Detailed biophysical characteristics for each WEN and JER site are provided in Table 3 of Webb et al. (2016a) and Table 1 of Webb et al. (2016b), respectively. Although there are three other JER sites (sites 1, 2, and 5), only data from JER Site 3 and JER Site 4 are provided here and used for the analysis.  

**Minute-frequency datasets:**<br/>
**TIMESTAMP** <- Datetime stamp in YYYY-mm-dd HH:MM:SS format (local standard time)<br/>
**CldCvrFrac** <- Cloud cover fraction<br/>
**SolarZen** <- Solar zenith angle (degrees) <br/>
**Albedo** <- Average 1min surface albedo measured by net radiometer<br/>
**Rainfall** <- Total rainfall accumulated over 1 minute (mm)<br/>
**AirTemp_400cm** <- Average 1min air temperature 4m above ground level (deg Celcius)<br/>
**AirTemp_200cm** <- Average 1min air temperature 2m above ground level (deg Celcius)<br/>
**WindDir_480cm** <- Average 1min wind direction 4.8m above ground level (deg from North)<br/>
**WindSpd_480cm** <- Average 1min wind speed 4.8m above ground level (m s^-1)<br/>
**WindSpd_240cm** <- Average 1min wind speed 2.4m above ground level (m s^-1)<br/>
**WindSpd_140cm** <- Average 1min wind speed 1.4m above ground level (m s^-1)<br/>
**WindSpd_70cm** <- Average 1min wind speed 0.7m above ground level (m s^-1)<br/>
**WindSpd_15AVG_480cm** <- Average 15min wind speed 4.8m above ground level (m s^-1)<br/>
**WindSpd_15AVG_240cm** <- Average 15min wind speed 2.4m above ground level (m s^-1)<br/>
**WindSpd_15AVG_140cm** <- Average 15min wind speed 1.4m above ground level (m s^-1)<br/>
**WindSpd_15AVG_70cm** <- Average 15min wind speed 0.7m above ground level (m s^-1)<br/>
**FV_regress** <- Friction velocity diagnosed from linear regression (m s^-1)<br/>
**z0_regress** <- Aerodynamic roughness length diagnosed from linear regression (m)<br/>
**z0_filt** <- Aerodynamic roughness length diagnosed from linear regression with filters applied (m)<br/>
**z0_daily** <- Average 24hour roughness length estimated from wind speed profile calculated from z0_filt (m)<br/>
**FV_pro** <- Wind speed profile-based friction velocity (m s^-1)<br/><br/>

**Daily datasets:**<br/>
**Date** <- Date stamp in YYYY-mm-dd format (local standard time)<br/>
**z0_pro** <- Daily average aerodynamic roughness length estimated from wind speed profile (m)<br/>
**SolarZenMin** <- Minimum solar zenith angle (degrees) <br/>
**TimeSolarZenMin** <- Time at which minimum solar zenith angle occured in HH:MM:SS format<br/>
**AlbedoSolarZenMin** <- Surface albedo measured by net radiometer when minimum solar zenith angle occured<br/>
**LandSatR** <- Surface reflectance obtained from 30m Landsat 8 cloud-free surface reflectance product (mm)<br/>
**Wns_rad** <- Rescaled normalized albedo determined from net radiometer<br/>
**Wns_modis** <- Rescaled normalized albedo determined from MODIS <br/>
**ustarUf_pro** <- Daily average normalized friction velocity determined from wind speed profile<br/>
**uTstarUh_rad** <- Daily normalized total friction velocity determined from net radiometer<br/>
**usstarUh_rad** <- Daily normalized friction velocity at the soil surface determined from net radiometer<br/>
**uTstarUh_rad_filt** <- Filtered daily normalized total friction velocity determined from net radiometer<br/>
**usstarUh_rad_filt** <- Filtered daily normalized friction velocity at the soil surface determined from net radiometer<br/>
**uTstarUh.modis** <- Daily normalized total friction velocity determined from MODIS<br/>
**usstarUh.modis** <- Daily normalized friction velocity at the soil surface determined from MODIS<br/><br/>

with "YYYY" representing the year, "m" the month, "d" the day of the month, "H" the hour of the day in 24-hour time, "MM" the minute of the hour, and "SS" the seconds.

MODIS albedo data are derived from the daily 500m MCD43A3 product.

Cloud cover fraction data were collected by the Las Cruces, NM ASOS station available online via https://mesonet.agron.iastate.edu/request/download.phtml?network=NM_ASOS. Following METAR reporting standards, we assumed  clear skies (CLR) = 0/8 cloud cover, few clouds (FEW) = 2/8 cloud cover, scattered clouds (SCT) = 4/8 cloud cover, broken clouds (BKN) = 6/8 cloud cover, overcast (OVC) = 8/8 cloud cover, and 8/8 cloud cover when vertical visibility obscrurants (VV) were reported.

Filtered daily normalized total and soil surface friction velocity values only include rainfree and clear sky time periods in their calculatiton.    

FV_pro is estimated using z0_daily, WindSpd_15AVG_480cm, and the law of the wall equation.

## References
Webb, N. P., Herrick, J. E., Van Zee, J. W., Courtright, E. M., Hugenholtz, C. H., Zobeck, T. M., Okin, G. S., Barchyn, T. E., 
Billings, B. J., Boyd, R., Clingan, S. D., Cooper, B. F., Duniway, M. C., Derner, J. D., Fox, F. A., Havstad, K. M., 
Heilman, P., LaPlante, V., Ludwig, N. A., Metz, L. J., Nearing, M. A., Norfleet, M. L., Pierson, F. B., Sanderson, M. A., 
Sharratt, B. S., Steiner, J. L., Tatarko, J., Tedela, N. H., Toledo, D., Unnasch, R. S., Van Pelt, R. S. and Wagner, L.: The 
National Wind Erosion Research Network: Building a standardized long-term data resource for aeolian research, modeling and land management, Aeolian Res., 22, 23–36, doi:10.1016/j.aeolia.2016.05.005, 2016a.

Webb, N. P., Galloza, M. S., Zobeck, T. M. and Herrick, J. E.: Threshold wind velocity dynamics as a driver of aeolian sediment mass flux, Aeolian Res., 20, 45–58, doi:10.1016/j.aeolia.2015.11.006, 2016b.
