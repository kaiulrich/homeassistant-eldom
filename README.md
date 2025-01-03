# Eldom Integration For Home Assistant

Connect your [Eldom](https://eldominvest.com/en/index.html) devices to Home Assistant and operate them via Eldom's Cloud APIs with [pyeldom](https://github.com/qbaware/pyeldom).

![eldom-integration](https://github.com/user-attachments/assets/d058d86b-0796-4d2f-b686-e9d4312ecd76)

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/danielgospodinow)

---

## Features

This integration allows you to control Eldom devices via Home Assistant.

Note that there's only one way to control your Eldom devices - via their Cloud APIs. There's no support for local network control.

### Supported devices

#### Flat boilers

- Operational mode selection
  - `Electric` (corresponds to "Heating")
  - `Eco` (corresponds to "Smart")
  - `High Demand` (corresponds to "Study")
  - `Off`
- Set target temperature
- Display current temperature
- Enable `Powerful mode` switch (only works while `Eco` mode is enabled)
- Display sensors
  - Heater is currently on/off
  - Day energy consumption
  - Night energy consumption
  - Saved energy

#### Smart boilers

- Operational mode selection
  - `Electric` (corresponds to "Heating")
  - `Eco` (corresponds to "Smart")
  - `High Demand` (corresponds to "Study")
  - `Off`
- Set target temperature
- Display current temperature
- Enable `Powerful mode` switch (only works while `Eco` mode is enabled)
- Display sensors
  - Heater is currently on/off
  - Day energy consumption
  - Night energy consumption
  - Saved energy

#### (Experimental) Convector heaters

- Operational mode selection
  - `Heat`
  - `Off`
- Set target temperature
- Display current temperature

### Showcase

![Flat boiler detailed view](./docs/flat-boiler-detailed-view-new.png)

![Flat boiler main view](./docs/flat-boiler-main-view-new.png)

## Installation

### HACS Installation

1. Open HACS.
2. Select `Integrations`, then select the 3-dots in the upper-right corner, then select `Custom Repositories`.
3. Put the reposity URL in the `Repository` field, then select `Integration` in the `Category` dropdown list and click `Add`.
4. Now, you can search for `Eldom` in HACS and install the integration.
5. After the installation, you need to restart Home Assistant.
6. Now, you can proceed with [Usage](#usage).

### Custom components

1. Download or clone the integration to your local machine.
2. Navigate to the `custom_components` directory in your Home Assistant installation directory.
3. Copy the folder `custom_components/eldom` from the downloaded integration to the Home Assistant `custom_components` directory.
4. Restart Home Assistant.

## Usage

- After installation, go to `Settings > Devices & services > Add integration` and search for `Eldom`.
- Provide an Eldom account `email` and `password` and click `Submit`.
