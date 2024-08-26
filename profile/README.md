# [Imeon Energy](https://imeon-energy.com/) Inverters for [Home Assistant](https://www.home-assistant.io/)

![screenshot-1](https://github.com/Imeon-Inverters-for-Home-Assistant/imeon-integration-extras/blob/master/dashboard-1.png "Front page")

This organisation contains the different repositories needed to port Imeon Inverters to Home Assistant systems.

## [imeon-integration](https://github.com/Imeon-Inverters-for-Home-Assistant/imeon-integration)

This is a custom integration that allows to communicate with the inverter through an intermediate API. Creates **HUBs** of **Sensors** and **Text** entities allowing to track each setting or power value with low latency. Also provides custom **Services** to change settings manually or through frontend and automations.

## [imeon-integration-extras](https://github.com/Imeon-Inverters-for-Home-Assistant/imeon-integration-extras)

Dashboard example meant to be paired with **imeon-integration**. Just contains .yaml files for Home Assistant Frontend and provides a decent base for anyone wanting to make a surpervision screen. Depends on https://github.com/RomRider/apexcharts-card for graphs and some gauges.

## [inverter-api](https://github.com/Imeon-Inverters-for-Home-Assistant/inverter-api)

A standalone API to collect data from the inverters. Uses HTTP POST/GET. It is used by **imeon-integration** to gather data from the inverter and send grouped commands to change settings. 

*You can also use this, alone, as a mean of gathering data, perhaps in another Smart Home system akin to Home Assistant.*

