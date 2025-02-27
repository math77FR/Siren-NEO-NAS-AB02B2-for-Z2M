
# NEO Siren Trigger Blueprint

This repository contains a Home Assistant blueprint for triggering a NEO NAS-AB02B2 siren using Zigbee2MQTT.

## Description
The NEO Siren Trigger Blueprint allows you to easily configure and control a NEO NAS-AB02B2 siren within Home Assistant. The blueprint sends MQTT commands to set the melody, volume, and duration of the siren alarm and restores the initial settings after the alarm is completed.

## Features
- Select a melody from 18 predefined options
- Set the volume level (low, medium, high)
- Define the duration of the siren alarm (1 to 1800 seconds)
- Automatically restores the siren's original melody and volume

## Prerequisites
- Home Assistant installed and running
- Zigbee2MQTT integration configured
- A NEO NAS-AB02B2 siren connected to your Zigbee network

## Installation
1. Copy the `blueprint.yaml` file to your Home Assistant `config/blueprints/script` directory.
2. Reload blueprints in Home Assistant.
3. Create a new script using the "NEO Siren Trigger Blueprint".

## Configuration
When setting up the blueprint, you need to provide:
- The siren device (via device selector)
- The melody to play
- The duration of the alarm
- The volume level

## Example Usage
```yaml
script:
  trigger_siren_example:
    use_blueprint:
      path: yourusername/neo_siren_trigger_blueprint.yaml
      input:
        device_id: 'your_device_id'
        melody: '7'  # Red Alert
        duration: 10
        volume: 'high'
```

## License
This project is licensed under the MIT License.
