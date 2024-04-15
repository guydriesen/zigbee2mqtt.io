---
title: "Bosch BSD-2 control via MQTT"
description: "Integrate your Bosch BSD-2 via Zigbee2MQTT with whatever smart home infrastructure you are using without the vendor's bridge or gateway."
addedAt: 2023-03-30T17:14:41
pageClass: device-page
---

<!-- !!!! -->
<!-- ATTENTION: This file is auto-generated through docgen! -->
<!-- You can only edit the "Notes"-Section between the two comment lines "Notes BEGIN" and "Notes END". -->
<!-- Do not use h1 or h2 heading within "## Notes"-Section. -->
<!-- !!!! -->

# Bosch BSD-2

|     |     |
|-----|-----|
| Model | BSD-2  |
| Vendor  | [Bosch](/supported-devices/#v=Bosch)  |
| Description | Smoke alarm detector |
| Exposes | smoke, battery, battery_low, test, intruder_alarm_state, smoke_alarm_state, linkquality |
| Picture | ![Bosch BSD-2](https://www.zigbee2mqtt.io/images/devices/BSD-2.png) |


<!-- Notes BEGIN: You can edit here. Add "## Notes" headline if not already present. -->
## Notes
### Pairing
- Before starting the pairing process the device's install code needs to be added to Zigbee2MQTT. Scan the QR code printed on the bottom of the device with the camera of your mobile phone and copy the received value (Attention: The install code printed in plain text on the device is not sufficient!) 
- The install code can be found inside the device before attaching it to the mounting plate
- Add this install code under Settings -> Tools -> Add install code
<!-- Notes END: Do not edit below this line -->




## Exposes

### Smoke (binary)
Indicates whether the device detected smoke.
Value can be found in the published state on the `smoke` property.
It's not possible to read (`/get`) or write (`/set`) this value.
If value equals `true` smoke is ON, if `false` OFF.

### Battery (numeric)
Remaining battery in %, can take up to 24 hours before reported.
Value can be found in the published state on the `battery` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `0` and the maximum value is `100`.
The unit of this value is `%`.

### Battery low (binary)
Indicates if the battery of this device is almost empty.
Value can be found in the published state on the `battery_low` property.
It's not possible to read (`/get`) or write (`/set`) this value.
If value equals `true` battery low is ON, if `false` OFF.

### Test (binary)
Indicates whether the device is being tested.
Value can be found in the published state on the `test` property.
It's not possible to read (`/get`) or write (`/set`) this value.
If value equals `true` test is ON, if `false` OFF.

### Intruder alarm state (binary)
Toggle the intruder alarm on or off.
Value can be found in the published state on the `intruder_alarm_state` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"intruder_alarm_state": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"intruder_alarm_state": NEW_VALUE}`.
If value equals `ON` intruder alarm state is ON, if `OFF` OFF.

### Smoke alarm state (binary)
Toggle the smoke alarm on or off.
Value can be found in the published state on the `smoke_alarm_state` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"smoke_alarm_state": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"smoke_alarm_state": NEW_VALUE}`.
If value equals `ON` smoke alarm state is ON, if `OFF` OFF.

### Linkquality (numeric)
Link quality (signal strength).
Value can be found in the published state on the `linkquality` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `0` and the maximum value is `255`.
The unit of this value is `lqi`.

