---
title: Blue Current
description: Instructions on how to integrate Blue Current charge points within Home Assistant.
ha_category:
  - Sensor
  - Switch
  - Car
ha_release: 2021.10
ha_iot_class: Cloud Push
ha_config_flow: true
ha_codeowners:
  - '@Floris272'
ha_domain: bluecurrent
ha_platforms:
  - sensor
  - switch
---

[BlueCurrent](https://www.bluecurrent.nl/) is an Dutch company that makes electric car chargers.

The Blue Current integration platform can be used to access data from your charge point(s).

## Prerequisites

1. Login to the BlueCurrent portal
2. Generate an api token

{% include integrations/config_flow.md %}

## Sensor

The Blue Current integration provides the following sensors:

### charge point sensors

- current phase 1
- current phase 2
- current phase 3
- total current
- voltage phase 1
- voltage phase 2
- voltage phase 3
- total voltage
- energy usage in kWh
- session start time
- session stop time
- offline since
- total cost in EUR
- vehicle status
- activity

### grid sensors

- grid current phase 1
- grid current phase 2
- grid current phase 3
- grid total current

## Switch

The Blue Current integration provides the following switches:

- available
- plug_and_charge
- public_charging