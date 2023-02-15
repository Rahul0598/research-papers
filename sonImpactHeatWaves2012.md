The study investigated the association between heat waves and mortality in seven major cities in Korea (Seoul, Busan, Daegu, Incheon, Gwangju, Daejeon, and Ulsan). The authors used a time-series approach to estimate the association between heat waves and mortality in each city, adjusting for potential confounding factors such as air pollution, day of the week, and season. They also examined whether the association varied by age and cause of death.

**Lag effects information:** The study examined the effects of heat waves on mortality with different lag periods, ranging from 0 to 7 days.

**Statistical methods:** The authors used a time-series regression model with a quasi-Poisson distribution to estimate the association between heat waves and mortality, adjusting for potential confounding factors. They used distributed lag non-linear models (DLNMs) to examine the effects of heat waves with different lag periods. They also performed stratified analyses by age and cause of death.

**Data sources:** The study used daily data on mortality, temperature, and air pollution in seven major cities in Korea for the period from 2000 to 2009. The mortality data were obtained from the Korean National Statistical Office, and the temperature and air pollution data were obtained from the Korean Meteorological Administration and the National Institute of Environmental Research, respectively.
 
**Algorithms used:** The authors used the DLNM package in R to fit the time-series regression models with a quasi-Poisson distribution. They also used the same package to fit the DLNMs to examine the effects of heat waves with different lag periods.
 
**How they distinguished between heat wave and non-heat wave days:** The authors used the definition of a heat wave as the period of at least two consecutive days with a daily maximum temperature exceeding the 95th percentile of the daily maximum temperature for the reference period (1961-1990). They defined non-heat wave days as all other days.
