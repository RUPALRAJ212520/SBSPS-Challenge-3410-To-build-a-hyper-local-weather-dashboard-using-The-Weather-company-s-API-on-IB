https://drive.google.com/file/d/1089mtslKbJltCM86FgJNkungaLYktXCA/view?usp=sharing (VIDEO PRESENTATION OF THIS PROJECT)

https://drive.google.com/file/d/1aNwiFdD3WfBvF5muU4_Qh32u4r_rXAyu/view?usp=sharing ( PROJECT REPORT)









# node-red-contrib-twc-weather
Node-RED nodes for The Weather Company and Weather Underground Personal Weather Station APIs

These nodes replace the depreciated **node-red-node-weather-underground** with new TWC apis for querying [wunderground.com](https://wunderground.com) Personal Weather Station (PWS) data.

The set of nodes in this package implement the [APIs for Personal Weather Station Contributors](https://docs.google.com/document/d/1eKCnKXI9xnoMGRRzOL1xPCBihNV2rOet08qpE_gArAY).

The Weather Company provides [TWC Weather Data Packages](https://business.weather.com/products/weather-data-packages) that are available for purchase. Node-RED nodes in this package implement select API services.

## Install

Either use the Editor - Menu - Manage Palette - Install option, or run the following command in your Node-RED user directory (typically `~/.node-red`).
```
$ npm install node-red-contrib-twc-weather
```

## Usage

Register your Personal Weather Station at [wunderground](https://www.wunderground.com/member/devices) and copy your PWS Station ID and API Key into these Node-RED nodes.

![wunderground mydevices](wunderground-mydevices.png)

## node-red-contrib-twc-weather Nodes

This Node-RED package creates six PWS nodes in your Node-RED palette.
- **pws observations** - Personal Weather Station (PWS) Current Conditions returns the current conditions observations.
- **pws historical** - Personal Weather Station (PWS) Historical Data returns the historical PWS data for a single date ( hourly data, summary data for the entire day, or all records )
- **pws forecast** - The Daily Forecast API is sourced from the The Weather Company Forecast system. This TWC API returns the 5 Day Daily weather forecast.
- **pws 7 day summary** - Personal Weather Station (PWS) Daily Summary Historical Observations returns the 7 day summary of daily observations.
- **pws 7 day hourly** - Personal Weather Stations (PWS) Hourly Historical Observations returns the hourly records for each days observations report.
- **pws 1 day all** - Personal Weather Station (PWS) Rapid Historical Observations returns all of the observations records for a specific date.

This Node-RED package creates TWC nodes in your Node-RED palette.
- **TWC Daily Forecast** - (3, 5, 7, 10, 15 Day) Daily Forecast API from the TWC Core Weather Data Package.
- **TWC Health Forecast** - The Cognitive Health Forecast API provides forecast data for the risk of allergy, migraine, cold and flu, or pain for a given location and for a period of one to 15 days in advance.
- **TWC Nowcast** - The short range Nowcast Forecast API provides a text summary of the weather forecast for the next 6 hour period for today.


