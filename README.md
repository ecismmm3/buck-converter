# buck-converter
currently working on a <40V to 5V buck converter

## Electrical Components

- LM2596S-5.0 IC
- Screwdriver Terminal Blocks (x2)
- Capacitors (C1 = 470uF 50V, C2 = 330uF 25V)
- Inductor (68 uH)
- 1N5820 Schottky Diode (x1)

## Testing (simulation)

- 10 ohm resistor connected as a test load between OUTPUT and GND

Schematic + SPICE Directives (custom part in ./LTSpice):
<img width="1753" height="528" alt="image" src="https://github.com/user-attachments/assets/67cac206-5660-4d0e-945d-50635854c98d" />

Voltage at OUT Pin (duty cycle):
<img width="1896" height="372" alt="image" src="https://github.com/user-attachments/assets/b75603d7-7a96-4b51-8652-1ea4cf2c1884" />

Voltage Plots:
<img width="1887" height="367" alt="image" src="https://github.com/user-attachments/assets/1cc51157-2584-4d08-9320-0a828578101e" />
- Green: Input
- Blue: output
- Red: reference voltage (at FB)

Current Plots:
<img width="1897" height="373" alt="image" src="https://github.com/user-attachments/assets/73d0339c-3d1b-4993-b1f6-c24730b2a020" />
<img width="1767" height="372" alt="image" src="https://github.com/user-attachments/assets/69f55423-3fd3-4164-b8aa-a48e892b730f" />

- Blue: Inductor
  - Load (0.5A) + Capacitor
- Red: Capacitor
  - Positive: charging
  - Negative: discharging to supply load
- Green: Diode
  - Equal to (carries) the inductor current when the switch is open, 0A when its on










