# RS485Expander

## Overview

RS485Expander is a non-isolated 9-port RS485 hub designed to expand RS485 networks efficiently and cost-effectively. This device allows you to connect multiple RS485 devices together, making it ideal for industrial automation, building management systems, and other applications where robust multi-drop RS485 communication is required.

## Features

- **9 RS485 Ports**: Connect up to 8 slave devices and 1 master device.
- **Non-Isolated Design**: For cost-sensitive applications where isolation is not required.
- **Compact PCB**: Space-saving design for easy integration into control panels.
- **Robust Communication**: Supports standard RS485 multi-drop protocol.
- **LED Indicators**: Visual feedback for power and communication status (if available in the hardware).

## Typical Applications

- Building automation
- Industrial control systems
- SCADA networks
- Sensor networks
- Data acquisition systems

## Hardware Description

The RS485Expander consists of a PCB with 9 RS485 transceiver circuits. Each port is connected in parallel to support multi-drop communication. The hub is powered via a standard DC jack or terminal block (specify voltage if known). The board is not galvanically isolated; ensure all connected devices share a common ground.

## Schematic & PCB

- Schematic and PCB design files are available in the [`hardware`](./hardware) directory.
- Supported design software: (e.g., KiCAD, Eagle, Altium) *(specify if known)*

## Getting Started

1. **Connect Power**: Apply the required DC voltage (specify rating, e.g., 12V DC).
2. **Connect RS485 Devices**: Use twisted pair cables for the A/B lines and connect common ground.
3. **Termination Resistors**: Add termination resistors at the end devices if required by your network topology.
4. **Test Communication**: Use your RS485 master device to verify communication with all slave ports.

## Pinout

| Port | Description      |
|------|-----------------|
| 1-8  | Slave device    |
| 9    | Master device   |
| GND  | Common ground   |

*(Customize for your PCB if different)*

## Safety & Notes

- **Not Isolated**: Do NOT use in applications where isolation is required between ports.
- **Grounding**: Ensure all devices share a common ground to avoid communication errors.
- **Cable Length**: RS485 supports up to 1200 meters total cable length, but keep stubs as short as possible.

## License

This project is licensed under the MIT License. See [`LICENSE`](./LICENSE) for details.

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## Contact

For questions or support, please contact [repo owner](https://github.com/eldar6776).
