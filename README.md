# Home Assistant Custom Component: Slovenian Energy Tariff Calculator (Omrežnina)

This custom component for Home Assistant calculates the current network fee tariff based on the energy distributor's rates in Slovenia. It considers various factors such as the date, whether it's a weekend, a public holiday, or a specific season of the year to calculate the tariff.

## Features

- Calculates current energy tariff based on date and time.
- Automatically identifies weekends and Slovenian public holidays.
- Adjusts tariffs for high and low seasons.

## Installation
Ensure you have [HACS](https://hacs.xyz/) installed in your Home Assistant.

### Method 1 _(easiest)_:
[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=devdems&repository=home-assistant-network-tariff&category=plugin)

### Method 2: 

1. **Download the Custom Component**
   - Download the files from the repository.
   
2. **Copy to Your Custom Components Directory**
   - Copy the downloaded files into the `custom_components/elektro_network_tariff` directory in your Home Assistant configuration directory.

3. **Restart Home Assistant**
   - Restart your Home Assistant instance to load the new component.

## Configuration

After installation, you need to add the component to your Home Assistant configuration. Edit your `configuration.yaml` file and add the following configuration:

```yaml
sensor:
  - platform: elektro_network_tariff
