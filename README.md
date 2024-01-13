# ESP Temperature Sensor

<div align="center">
    <table align="center">
        <td>
            <img
                align="center"
                src="https://raw.githubusercontent.com/jepnoda/ESP-Temperature-Sensor/main/device-enclosed.jpg"
                 alt="device-enclosed"
            />
        </td>
        <td>
            <img
            align="center"
            src="https://raw.githubusercontent.com/jepnoda/ESP-Temperature-Sensor/main/device-opened.jpg"
            alt="device-opened"
            />
        </td>
    </table>
</div>

A device built with an AHT20 Temperature/Humidity Module, an ESP32-S2 Microcontroller, SSD1306 OLED Display Module, and ESPHome Custom Firmware that can be integrated into Home Assistant to monitor the temperature and relative humidity of the surroundings.

## Features

- Temperature Monitoring
- Relative Humidity Monitoring
- With Display (Temperature and relative humidity are shown in real time)

## Prerequisites

This device was built with [ESPHome](https://esphome.io/) and is intended to work with [Home Assistant.](https://www.home-assistant.io/)

### Modules

- [ESP32-S2 Mini](https://shopee.ph/ESP32-S2-Mini-V1.0.0-LOLIN-WIFI-IOT-Board-based-ESP32-S2FN4R2-ESP32-S2-4MB-FLASH-2MB-PSRAM-MicroPython-Arduino-Compatible-i.517103615.20023297921?sp_atk=c3f0aed0-2a24-4854-b7e6-989adb8a48c8&xptdk=c3f0aed0-2a24-4854-b7e6-989adb8a48c8)
- [AHT20 Temperature and Humidity Measurement Module](https://shopee.ph/AHT10-AHT20-AHT30-High-Precision-Digital-Temperature-and-Humidity-Sensor-Measurement-Module-I2C-Communication-Replace-SHT20-i.580325202.15490162049?sp_atk=ad350830-e188-4e7f-aa8b-27aa14556745&xptdk=ad350830-e188-4e7f-aa8b-27aa14556745)
- [SSD1306 OLED Display Module](https://shopee.ph/0.96-inch-128x64-pixels-SSD1306-OLED-Display-Module-i.237034143.6548465016?sp_atk=789abb04-2939-47aa-a893-fea9c23f6f77&xptdk=789abb04-2939-47aa-a893-fea9c23f6f77)

## Getting Started

### Pictorial Diagram

![pictorial-diagram](https://raw.githubusercontent.com/jepnoda/ESP-Temperature-Sensor/main/pictorial-diagram.png)

❗❗❗ For [ESP32-S2 Mini](https://www.wemos.cc/en/latest/s2/s2_mini.html), use `IO33` for `SDA` and `IO35` for `SCL`.

| AHT20 Pin | SSD1306 OLED Pin | ESP32 Pin |
| :---: | :---: | :---: |
| SDA | SDA | D21 |
| SCL | SCL | D22 |
| VCC | VCC | 3V3 |
| GND | GND | GND |

---

1. Ensure [ESPhome](https://esphome.io/guides/getting_started_hassio) and [File Editor](https://github.com/home-assistant/addons/blob/master/configurator/DOCS.md) add-ons are installed on your [Home Assistant](https://www.home-assistant.io/getting-started/) instance.
2. Ensure that your ESPHome `secrets.yaml` file is up to date.
3. Using the File Editor add-ons, upload the `esp-temperature-sensor.yaml` config file along with `materialdesignicons-webfont.ttf` font file on the `config/esphome/`.
4. Using the ESPHome dashboard, modify the `esp-temperature-sensor.yaml` and replace the **redacted** part of the config file.
5. **Build** and **upload** the firmware to your device.
6. Now, you can [integrate](https://www.home-assistant.io/getting-started/concepts-terminology/) the device into your Home Assistant.

---

### Operational Device

![device-running](https://raw.githubusercontent.com/jepnoda/ESP-Temperature-Sensor/main/device-running.jpg)
