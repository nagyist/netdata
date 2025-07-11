<!--startmeta
custom_edit_url: "https://github.com/netdata/netdata/edit/master/src/collectors/proc.plugin/integrations/power_supply.md"
meta_yaml: "https://github.com/netdata/netdata/edit/master/src/collectors/proc.plugin/metadata.yaml"
sidebar_label: "Power Supply"
learn_status: "Published"
learn_rel_path: "Collecting Metrics/Linux Systems/Power Supply"
most_popular: False
message: "DO NOT EDIT THIS FILE DIRECTLY, IT IS GENERATED BY THE COLLECTOR'S metadata.yaml FILE"
endmeta-->

# Power Supply


<img src="https://netdata.cloud/img/powersupply.svg" width="150"/>


Plugin: proc.plugin
Module: /sys/class/power_supply

<img src="https://img.shields.io/badge/maintained%20by-Netdata-%2300ab44" />

## Overview

This integration monitors Power supply metrics, such as battery status, AC power status and more.



This collector is supported on all platforms.

This collector supports collecting metrics from multiple instances of this integration, including remote instances.


### Default Behavior

#### Auto-Detection

This integration doesn't support auto-detection.

#### Limits

The default configuration for this integration does not impose any limits on data collection.

#### Performance Impact

The default configuration for this integration is not expected to impose a significant performance impact on the system.


## Metrics

Metrics grouped by *scope*.

The scope defines the instance that the metric belongs to. An instance is uniquely identified by a set of labels.



### Per power device



Labels:

| Label      | Description     |
|:-----------|:----------------|
| device | TBD |

Metrics:

| Metric | Dimensions | Unit |
|:------|:----------|:----|
| powersupply.capacity | capacity | percentage |
| powersupply.power | power | W |
| powersupply.charge | empty_design, empty, now, full, full_design | Ah |
| powersupply.energy | empty_design, empty, now, full, full_design | Wh |
| powersupply.voltage | min_design, min, now, max, max_design | V |



## Alerts


The following alerts are available:

| Alert name  | On metric | Description |
|:------------|:----------|:------------|
| [ power_supply_capacity ](https://github.com/netdata/netdata/blob/master/src/health/health.d/power_supply_capacity.conf) | powersupply.capacity | percentage of remaining power supply capacity |


## Setup

### Prerequisites

No action required.

### Configuration

#### File

There is no configuration file.
#### Options



There are no configuration options.

#### Examples
There are no configuration examples.


