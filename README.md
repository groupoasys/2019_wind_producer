# Readme of the  2019_wind_producer repository 
Power systems data (2015-2019) used in the numerical case study of the [paper] published on IEEE Transactions on Power Systems. The data includes relevant forecasts of DK1 bidding zone and wind power production forecasts of nearby areas. Day-ahead market prices of DK1 are also included. 

## Dataset Content 
This section describes in detail the data series of the only data file in the repository: dataset_wind_europe_2015_2019.csv

### Time

TimeUTC: UTC time

hour of day (hourXX): dummy variable equal 1 when TimeUTC.hour == hourXX (24 series).

day_of_weak (monday, tusday, …): dummy variable equal 1 when TimeUTC.dayofweek == day_of_week (7 series).

### Data from Energinet

Data source: [Energinet] and [Nord Pool]

SpotPriceEUR: (euros) Spot price in Euros for DK1 (Nordpool).

BalancingPowerPriceDownEUR: (euros) Balancing price of downward regulataion for DK1.

BalancingPowerPriceUpEUR: (euros) Balancing price of upward regulation for DK1.

### Data from Entsoe

Data source: [ENTSO-e Transparency Platform]

Warning! The day ahead data may not follow the Manual of Procedure of the Transparency Platform and may be uploaded after the 18.00 Brussels time deadline of day D-1. The data is sometimes updated afterwards, even months later.

XX_won_real: (MWh) actual onshore wind production of bidding zone XX. 

XX_won_da: (MWh) day ahead (before 18.00 Brussels time day D-1) onshore wind production of bidding zone XX. 

XX_woff_real: (MWh) actual offshore wind production of bidding zone XX.

XX_woff_da: (MWh) day ahead (before 18.00 Brussels time day D-1) offshore wind production of bidding zone XX.

DK1_SchedGen: (MWh) Scheduled generation for DK1. 

DK1_SolarDahead: (MWh) Solar production forecasted for DK1. (before 18.00 Brussels time day D-1)

DK1_TotalLoadDahead: (MWh) Total Load forecasted for DK1. (before 18.00 Brussels time day D-1)

### Other data

DK1_FM3_output: (MWh) Output of the first step optimization problem tailored to forecasting as described in the [paper].

## Useful related websites

[Nord Pool]

[Energinet]

[ENTSO-e Transparency Platform]

[The Wind Power]

## How to cite the paper?

If you want to cite this [paper] you can use the following text:
```
 M. A. Muñoz, J. M. Morales y S. Pineda, Feature-driven Improvement of Renewable Energy Forecasting and Trading, IEEE Transaction on Power Systems, 2020.
```
or the .bib version:

```
@article{Munoz2020feat,
  title={Feature-driven Improvement of Renewable Energy Forecasting and Trading},
  author={Mu{\~n}oz, Miguel Angel and Morales, Juan Miguel and Pineda, Salvador},
  journal={IEEE Transactions on Power Systems},
  year={2020},
  volume={},
  number={},
  pages={},
  publisher={IEEE},
  keywords={Electricity markets; Machine Learning; Optimization; Renewable energy forecasting and trading; Windpower},
  doi={10.1109/TPWRS.2020.2975246},
}
```

## Developed by 

 * [Miguel Angel Muñoz Diaz](https://www.researchgate.net/profile/Miguel_Munoz_Diaz) - miguelangeljmd@uma.es
 * [Juan Miguel Morales](https://www.researchgate.net/profile/Juan_Morales25) - juan.morales@uma.es
 * [Salvador Pineda](https://www.researchgate.net/profile/Salvador_Pineda) - spinedamorente@gmail.com
 * [OASYS group](http://oasys.uma.es) -  groupoasys@gmail.com

## Do you want to contribute?
 
Any feedback is welcome so feel free to ask or comment anything you want via a Pull Request in this repo.
 
## License
 
Please, see the LICENSE file.
    
[paper]: https://doi.org/10.1109/TPWRS.2020.2975246
[Energinet]: https://www.energidataservice.dk/en/dataset
[ENTSO-e Transparency Platform]: https://transparency.entsoe.eu/
[Nord Pool]: https://www.nordpoolgroup.com/Market-data1/Dayahead/Area-Prices/ALL1/Hourly/?view=table
[The Wind Power]: https://www.thewindpower.net/owner_en_107_rwe.php
