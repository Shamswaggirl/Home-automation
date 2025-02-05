# Node-RED Home Automation Simulation

## Introduction
IBM **Node-RED** is a flow-based programming tool that allows users to wire together hardware devices, APIs, and online services. In this project, **Node-RED** is used to simulate a **home automation setup** by creating multiple flows that control various home devices. The system operates using **MQTT protocol**, where messages are published and subscribed for seamless IoT communication.

## Features
- **Remote monitoring and control of home appliances**
- **Dashboard interface for real-time interaction**
- **Multiple flows for different home automation tasks**
- **Integration with MQTT for efficient message handling**

## Technology Stack
- **Platform:** Node-RED
- **Communication Protocol:** MQTT
- **Components:** MQTT IN, MQTT OUT, Switches, Gauges, Inject Nodes, Sliders, Buttons

## How It Works
### Accessing Node-RED Dashboard
- Open **Node-RED** using `IP:Port Number` as the website address.
- To access the dashboard, enter `IP:Port Number/ui`.

### Flows Implemented
#### 1. **Room Temperature Monitoring**
- Nodes Used: MQTT IN, Function, Gauge
- Functionality:
  - Temperature data is published through the **MQTT box**.
  - The dashboard displays temperatures of four rooms.

#### 2. **Light Control in Each Room**
- Nodes Used: MQTT OUT, Switches
- Functionality:
  - Users can turn **lights ON/OFF** via the dashboard.
  - The **MQTT box** subscribes to light status updates.

#### 3. **Fan Control in Each Room**
- Nodes Used: MQTT OUT, Switches
- Functionality:
  - Users can turn **fans ON/OFF** via the dashboard.
  - The **MQTT box** subscribes to fan status updates.

#### 4. **Multi-Device Control**
- Devices Controlled:
  - **Television, Home Theatre, Air Conditioner, Washing Machine, Car Shed Gate, Water Tank Level Indicator, Pet Feed Device**
- Nodes Used: MQTT IN, MQTT OUT, Inject, Slider, Button, Switch, Gauge
- Functionality:
  - Similar to light and fan control, users can operate devices via **publishing and subscribing messages** in MQTT.

## Benefits
- **Smart Home Automation** using Node-RED simulation
- **Minimal setup** required for IoT-based control
- **Scalable and customizable** for future home automation projects

## Installation & Setup
1. **Install Node-RED**: Follow installation steps from the [official website](https://nodered.org/).
2. **Set up MQTT Broker**: Use **Mosquitto** or any MQTT broker for message handling.
3. **Run Node-RED Flows**:
   - Import the provided Node-RED flows into your Node-RED instance.
   - Deploy the flows and test the dashboard.
4. **Access the Dashboard**:
   - Open `IP:Port Number/ui` in your web browser.
   - Control devices and monitor their status.

## Future Enhancements
- **Integration with voice assistants** (Alexa, Google Assistant)
- **AI-based automation** for predictive control
- **Cloud integration** for remote access

## Contribution
We welcome contributions! Feel free to submit pull requests or open issues for enhancements.

## License
This project is licensed under the **MIT License**.

## Contact
For any queries or collaboration opportunities, reach out via [GitHub Issues].

