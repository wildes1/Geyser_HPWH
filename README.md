# Heat Pump Water Heater Control

This project replaces the control board in a **Geyser 6000-3.0** heat pump water heater. It drops support for the electric water heater element.

## Relays

* **30A Relay:** Controls the compressor.
* **10A Relay:** Controls the fan.
* **10A Relay:** Controls the recirculating pump.

## Energy Monitoring

* **Sensor:** PZEM-004T V2 Energy Monitor.
* **Metrics:** Compressor voltage, current, and power.

## Plumbing & Flow

* **Pump:** Taco 006-BZ4 cartridge circulator.
* **Flow Rate:** ~8 CFM (equivalent to ~1 GPM / 60 GPH) at 4' head.
* **Adjustment:** Flow rate variable is adjustable in software.

## Temperature Sensors

1. Evaporator
2. Water Out
3. Internal Water Out
4. Internal Water In
5. Tank Top
6. Tank Bottom

## COP Calculation

Coefficient of Performance (COP) is calculated using the following inputs:

* `internal_water_in_temp`
* `internal_water_out_temp`
* `compressor_power`
* `flow_rate`
