# buck-converter
5V 1A DC-DC Buck Converter

## Electrical Components

- LM2596S-5.0 IC
- Screwdriver Terminal Blocks (x2)
- Capacitors (C1 = 470uF 50V, C2 = 330uF 25V)
- Inductor (33 uH)
- 1N5820 Schottky Diode (x1)

## Testing (simulation)

- 5 ohm test load (simulate 5V 1A)

Schematic + SPICE Directives (custom parts found in `LTSpice/`):
<img width="1266" height="351" alt="image" src="https://github.com/user-attachments/assets/25664018-9306-4a18-9770-3131c6dadc58" />

Voltage Plot:
<img width="1892" height="377" alt="image" src="https://github.com/user-attachments/assets/a06d0a99-8e39-4bd2-b95b-cc0c4b845f75" />

- Green: Input
- Blue: Output
- Red: duty cycle

Current Plot:
<img width="1892" height="372" alt="image" src="https://github.com/user-attachments/assets/f39ded14-42d9-4a2a-8241-5ec44d401dbb" />










