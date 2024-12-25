## Install ESPHome

1. Create a new venv and install ESPHome

```bash
python3 -m venv venv
source venv/bin/activate
```

2. Install ESPHome

```bash
pip install esphome
```

3. Copy `secrets.example.yaml` to `secrets.yaml` and fill in the values

```bash
cp secrets.example.yaml secrets.yaml
```

4. Run ESPHome

```bash
esphome run co2sensor.yaml
```

## M5Stack and Senseair S8 CO2 sensor integration

This is a simple integration of the Senseair S8 CO2 sensor with an M5Stack Basic Core. The M5Stack is connected to the Senseair S8 via UART. The M5Stack is running ESPHome and sends the CO2 sensor data to Home Assistant.

### M5Stack

The M5Stack is running ESPHome and sends the CO2 sensor data to Home Assistant. The M5Stack is connected to the Senseair S8 via UART.

### Senseair S8

The Senseair S8 is a CO2 sensor that is connected to the M5Stack via UART.

### Home Assistant

Home Assistant is used to display the CO2 sensor data from the M5Stack.

## Schematic

```
GPIO16 (RX) -> Senseair S8 (TX)
GPIO17 (TX) -> Senseair S8 (RX)
```
