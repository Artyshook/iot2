# <p style="display: flex; justify-content: space-between; align-items: center">Internet of things project <img src="logo.png" style="width: 200px"></p>
Internet of things is a project created by several students of the [Unicorn University](https://unicornuniversity.net/).

It is a smart building information system that collects information about essential characteristics of the buildings and after saves this information in the database.
## Prequisites
Supported version of NodeJS, installed NodeRED. Installed Raspberry Pie.
## Config
Plugins will be loaded automatically from [package.json](package.json) if you run `npm install`.
## How it works
Nodes with several sensors send information about concentration, voltage, temperature, relative humidity, illuminance, pressure, altitude and total VOC through WIFI to the gateway with the Raspberry Pie. Gateway then sends this information using the HTTP requests to the backend. There are several gateways with the certain amount of nodes connected to it. Each gateway has its own database for those nodes that are connected to it and there is a general database for all the nodes.