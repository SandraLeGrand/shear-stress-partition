# Shear Stress Partitioning
Data for estimating friction velocity and drag partition.

## Authors
* Nancy P. Ziegler (ERDC)
* Sandra L. LeGrand (ERDC)
* Nicholas P. Webb (USDA/NMSU) 
* Adrian Chappell (U. Cardiff)

## Created 
Winter 2018/2019

## Data

**Minute-frequency datasets:**<br/>
**TIMESTAMP** <- Datetime stamp in YYYY-mm-dd HH:MM:SS format<br/>
**CldCvrFrac** <- Cloud cover fraction<br/>
**SolarZen** <- Solar zenith angle (degrees) <br/>
**Albedo** <- Average 1min surface albedo measured by net radiometer<br/>
**Rainfall** <- Total rainfall accumulated over 1 minute (mm)<br/>
**AirTemp_500cm** <- Average 1min air temperature 5m above ground level (deg Celcius)<br/>
**AirTemp_200cm** <- Average 1min air temperature 2m above ground level (deg Celcius)<br/>
**WindDir_500cm** <- Average 1min wind direction 5m above ground level (deg from North)<br/>
**WindSpd_500cm** <- Average 1min wind speed 5m above ground level (m s^-1)<br/>
**WindSpd_240cm** <- Average 1min wind speed 2.4m above ground level (m s^-1)<br/>
**WindSpd_140cm** <- Average 1min wind speed 1.4m above ground level (m s^-1)<br/>
**WindSpd_70cm** <- Average 1min wind speed 0.7m above ground level (m s^-1)<br/>
**WindSpd_15AVG_500cm** <- Average 15min wind speed 5m above ground level (m s^-1)<br/>
**WindSpd_15AVG_240cm** <- Average 15min wind speed 2.4m above ground level (m s^-1)<br/>
**WindSpd_15AVG_140cm** <- Average 15min wind speed 1.4m above ground level (m s^-1)<br/>
**WindSpd_15AVG_70cm** <- Average 15min wind speed 0.7m above ground level (m s^-1)<br/>
**FV_regress** <- Friction velocity diagnosed from linear regression (m s^-1)<br/>
**z0_regress** <- Aerodynamic roughness length diagnosed from linear regression (m)<br/>
**z0_filt** <- Aerodynamic roughness length diagnosed from linear regression with filters applied (m)<br/>
**z0_daily** <- Average 24hour roughness length (m)<br/>
**FV_pro** <- Wind speed profile-based friction velocity (m s^-1)<br/><br/>

**Daily datasets:**<br/>
**Date** <- Date stamp in YYYY-mm-dd format<br/>
**z0_pro** <- Daily average aerodynamic roughness length (m)<br/>
**SolarZenMin** <- Minimum solar zenith angle (degrees) <br/>
**TimeSolarZenMin** <- Time at which minimum solar zenith angle occured in HH:MM:SS format<br/>
**AlbedoSolarZenMin** <- Surface albedo measured by net radiometer when minimum solar zenith angle occured<br/>
**LandSatR** <- Surface reflectance obtained from 30m Landsat 8 cloud-free surface reflectance product (mm)<br/>
**Wns_rad** <- Rescaled normalized albedo determined from net radiometer<br/>
**Wns_modis** <- Rescaled normalized albedo determined from MODIS <br/>
**ustarUf_pro** <- Daily average normalized friction velocity determined from wind speed profile<br/>
**uTstarUf_rad** <- Daily normalized total friction velocity determined from net radiometer<br/>
**usstarUf_rad** <- Daily normalized friction velocity at the soil surface determined from net radiometer<br/>
**uTstarUf_rad_filt** <- Filtered daily normalized total friction velocity determined from net radiometer<br/>
**usstarUf_rad_filt** <- Filtered daily normalized friction velocity at the soil surface determined from net radiometer<br/>
**uTstarUf.modis** <- Daily normalized total friction velocity determined from MODIS<br/>
**usstarUf.modis** <- Daily normalized friction velocity at the soil surface determined from MODIS<br/><br/>

with "YYYY" representing the year, "m" the month, "d" the day of the month, "H" the hour of the day in 24-hour time, "MM" the minute of the hour, and "SS" the seconds.
