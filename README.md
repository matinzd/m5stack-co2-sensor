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