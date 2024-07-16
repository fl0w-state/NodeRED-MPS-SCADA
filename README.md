# Node-RED MPS SCADA Project

![GitHub license](https://img.shields.io/github/license/your-username/Node-RED-MPS-SCADA)

This repository contains the Node-RED MPS SCADA project, including maintenance guides, Standard Operating Procedures (SOPs), JSON code for Node-RED flows, and PLC programs.

## Table of Contents

- [Introduction](#introduction)
- [Maintenance Guide](#maintenance-guide)
- [Standard Operating Procedures (SOP)](#standard-operating-procedures-sop)
- [Node-RED JSON Code](#node-red-json-code)
- [PLC Programs](#plc-programs)
- [License](#license)
- [Visuals](#visuals)

## Introduction

This project aims to develop a SCADA system using Node-RED for monitoring and controlling a Modular Production System (MPS). The project includes integration of multiple PLCs using FINS UDP and Modbus TCP protocols.

## Maintenance Guide

The maintenance guide provides detailed instructions on how to maintain the Node-RED MPS SCADA system.

### Regular Maintenance

1. **Check Node-RED Flows**: Ensure all flows are running without errors.
2. **Update Dependencies**: Regularly update Node-RED and installed nodes.
3. **Backup Flows**: Backup the current Node-RED flows.
4. **Inspect PLC Connections**: Verify all PLC connections are stable and functioning.

### Troubleshooting

1. **Node-RED Issues**: Refer to the Node-RED logs for error details.
2. **PLC Communication**: Check the PLC communication status and logs.
3. **Network Issues**: Ensure the network connectivity is stable and reliable.

## Standard Operating Procedures (SOP)

This section includes the SOPs for operating and managing the Node-RED MPS SCADA system.

### Starting the System

1. **Power On**: Turn on all PLCs and network devices.
2. **Launch Node-RED**: Start the Node-RED server.
3. **Load Flows**: Open the Node-RED dashboard and load the required flows.

### Shutting Down the System

1. **Stop Node-RED**: Gracefully stop the Node-RED server.
2. **Power Off**: Turn off all PLCs and network devices.

## Node-RED JSON Code

This section contains the JSON code for the Node-RED flows used in this project. The Node-RED flows are located in the [Node-RED](Node-RED) folder.

### Node-RED Modules in Use

The following Node-RED modules are used in this project:

1. **[node-red](https://flows.nodered.org/node/node-red)**
   - **Description**: A visual tool for wiring the Internet of Things.
   - ![node-red](https://user-images.githubusercontent.com/20273326/36631715-37a49f1e-196d-11e8-96eb-dc44c54c6f47.png)

2. **[node-red-contrib-filesystem](https://flows.nodered.org/node/node-red-contrib-filesystem)**
   - **Description**: Nodes to work with the filesystem in Node-RED.
   - ![filesystem](https://user-images.githubusercontent.com/3766663/62012107-45d22400-b179-11e9-9fb8-65db99044b8a.png)

3. **[node-red-contrib-influxdb](https://flows.nodered.org/node/node-red-contrib-influxdb)**
   - **Description**: Node-RED nodes to save and query data from an InfluxDB time series database.
   - ![influxdb](https://user-images.githubusercontent.com/3766663/61866893-9f423400-aecb-11e9-937c-b14c92e21043.png)

4. **[node-red-contrib-modbus](https://flows.nodered.org/node/node-red-contrib-modbus)**
   - **Description**: The all-in-one Modbus TCP and Serial contribution package for Node-RED.
   - ![modbus](https://user-images.githubusercontent.com/3766663/61866936-c0a31e00-aecb-11e9-8721-1e4ebd4555ee.png)

5. **[node-red-contrib-omron-fins](https://flows.nodered.org/node/node-red-contrib-omron-fins)**
   - **Description**: Node-RED nodes to interact with Omron PLCs using the FINS protocol.
   - ![omron-fins](https://user-images.githubusercontent.com/3766663/61866966-d285c100-aecb-11e9-8c60-f04a80c33e42.png)

6. **[node-red-dashboard](https://flows.nodered.org/node/node-red-dashboard)**
   - **Description**: A set of dashboard nodes for Node-RED.
   - ![dashboard](https://user-images.githubusercontent.com/20273326/36631715-37a49f1e-196d-11e8-96eb-dc44c54c6f47.png)

7. **[node-red-node-serialport](https://flows.nodered.org/node/node-red-node-serialport)**
   - **Description**: Node-RED nodes to talk to serial ports.
   - ![serialport](https://user-images.githubusercontent.com/3766663/61867004-f2b57f00-aecb-11e9-8222-b5f819362a67.png)

8. **[node-red-contrib-ui-led](https://flows.nodered.org/node/node-red-contrib-ui-led)**
   - **Description**: A Node-RED Dashboard user interface node that displays an LED status indicator.
   - ![ui-led](https://user-images.githubusercontent.com/37037323/43093223-71b8-11e8-8a9f-09ea2296ef47.png)

9. **[node-red-contrib-ui-media](https://flows.nodered.org/node/node-red-contrib-ui-media)**
   - **Description**: A Node-RED Dashboard UI media node.
   - ![ui-media](https://user-images.githubusercontent.com/20273326/37213058-d712da48-2382-11e8-8339-df839e1981f7.png)

10. **[node-red-contrib-ui-svg](https://flows.nodered.org/node/node-red-contrib-ui-svg)**
    - **Description**: A Node-RED Dashboard UI SVG node.
    - ![ui-svg](https://user-images.githubusercontent.com/20273326/37213115-f19dd19a-2382-11e8-9bcf-ff2e15e3423e.png)

## PLC Programs

This section contains the PLC programs used in this project. The PLC programs are provided in separate files within the `plc-programs` directory.

### Separating Station

- [example-plc-program-separating.ladder](plc-programs/Separating-Station/example-plc-program-separating.ladder)

### Storing Station

- [example-plc-program-storing.ladder](plc-programs/Storing-Station/example-plc-program-storing.ladder)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Visuals

![Node-RED Dashboard](images/node-red-dashboard.png)
