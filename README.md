# Trigger NEO Siren Script for Home Assistant

This repository provides two approaches to trigger a NEO NAS-AB02B2 siren using Zigbee2MQTT integration within Home Assistant.

## 🚦 Implementation Options

### 1. Call the Script Directly in Automations
In this approach, you call the script (`script_neo_siren.yaml`) directly within each automation that triggers the siren.

**Pros:**- Setup the siren parameters (melody, duration, volume) individually for each automation.- Greater flexibility if different automations require different siren behaviors.

**How to Implement:**- Add the script call in your automation and configure the parameters manually.

**Detailed Explanation:** [README_script.md](README_script.md)

### 2. Use a Blueprint to Create a Preconfigured Script
With this approach, you create a blueprint that generates a script with fixed parameters (melody, duration, volume, etc.). The generated script can then be used in multiple automations.

**Pros:**- Centralized setup of siren parameters in the blueprint.- Easier maintenance when using the siren in multiple automations.

**How to Implement:**- Define a blueprint that sets up the siren script.- Call the generated script in your automations.

**Detailed Explanation:** [README_Blueprint.md](README_Blueprint.md)

## 💡 Which Approach to Choose?
- **Option 1** is ideal if you need specific siren behaviors for different scenarios.
- **Option 2** is recommended if you want a consistent siren behavior across multiple automations with minimal maintenance.

## 📁 Installation
1. Copy the `script_neo_siren.yaml` file content.2. Paste it into your `scripts.yaml` file located in `/homeassistant/`.3. Verify the configuration in Home Assistant:   - Go to **Settings > System > Server Control > Check Configuration**.4. Restart Home Assistant to apply the changes.

## 🤝 Contributions
Feel free to submit issues, feature requests, or pull requests to enhance this script!

## 📜 License
This project is licensed under the MIT License.

---
Made with ❤️ by Mathieu
