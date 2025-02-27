# Trigger NEO Siren Script for Home Assistant

This repository contains a Home Assistant script to trigger a NEO NAS-AB02B2 siren using Zigbee2MQTT integration.

## 🚀 Features
- Trigger different melodies available on the NEO NAS-AB02B2 siren
- Configure volume and duration of the siren
- Automatically reset the siren to its initial melody and volume settings

## 📁 Installation
1. Copy the `script_neo_siren.yaml` file content.
2. Paste it into your `scripts.yaml` file located in `/homeassistant/`.
3. Verify the configuration in Home Assistant:
   - Go to **Settings > System > Server Control > Check Configuration**.
4. Restart Home Assistant to apply the changes.

## 🧰 Usage
- Navigate to **Settings > Automations and Scenes > Scripts** in Home Assistant.
- Find and run the `Trigger NEO Siren` script.
- Configure the siren, melody, volume, and duration as needed.

## 🔧 Configuration Options
- **Siren**: Select the NEO NAS-AB02B2 device.
- **Melody**: Choose from 18 available sounds (e.g., Für Elise, Big Ben, Police, Doorbell).
- **Duration**: Set the siren duration (1 to 1800 seconds).
- **Volume**: Set the volume (low, medium, high).

## 📝 Example Configuration
```yaml
play_neo_siren:
  alias: Trigger NEO Siren
  description: Trigger a NEO NAS-AB02B2 siren under Zigbee2MQTT
  mode: queued
  max: 10
```

## 🆘 Troubleshooting
- Ensure your NEO siren is properly integrated through Zigbee2MQTT.
- Verify MQTT messages using the Zigbee2MQTT logs.

## 🤝 Contributions
Feel free to submit issues, feature requests, or pull requests to enhance this script!

## 📜 License
This project is licensed under the MIT License.

---
Made with ❤️ by Mathieu
