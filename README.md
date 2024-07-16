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

This section contains the JSON code for the Node-RED flows used in this project. The flows are provided in the [Node-RED](Node-RED) directory.

### Node-RED Modules Used

- [node-red-dashboard](https://flows.nodered.org/node/node-red-dashboard)
- [node-red-node-ping](https://flows.nodered.org/node/node-red-node-ping)
- [node-red-node-serialport](https://flows.nodered.org/node/node-red-node-serialport)
- [node-red-node-sqlite](https://flows.nodered.org/node/node-red-node-sqlite)
- [node-red-contrib-context-monitor](https://flows.nodered.org/node/@ralphwetzel/node-red-context-monitor)
- [node-red-contrib-context-hook](https://flows.nodered.org/node/@sirimangus/node-red-contrib-context-hook)
- [node-red-contrib-context-nodes](https://flows.nodered.org/node/node-red-contrib-context-nodes)
- [node-red-contrib-ctrlx-automation](https://flows.nodered.org/node/node-red-contrib-ctrlx-automation)
- [node-red-contrib-filesystem](https://flows.nodered.org/node/node-red-contrib-filesystem)
- [node-red-contrib-influxdb](https://flows.nodered.org/node/node-red-contrib-influxdb)
- [node-red-contrib-modbus](https://flows.nodered.org/node/node-red-contrib-modbus)
- [node-red-contrib-nbrowser](https://flows.nodered.org/node/node-red-contrib-nbrowser)
- [node-red-contrib-omron-fins](https://flows.nodered.org/node/node-red-contrib-omron-fins)
- [node-red-contrib-ui-actions](https://flows.nodered.org/node/node-red-contrib-ui-actions)
- [node-red-contrib-ui-led](https://flows.nodered.org/node/node-red-contrib-ui-led)
- [node-red-contrib-ui-media](https://flows.nodered.org/node/node-red-contrib-ui-media)
- [node-red-contrib-ui-svg](https://flows.nodered.org/node/node-red-contrib-ui-svg)
- [node-red-node-ui-table](https://flows.nodered.org/node/node-red-node-ui-table)

## PLC Programs

This section contains the PLC programs used in this project. The PLC programs are provided in the [PLC Programs](PLC-Programs) directory, divided into the following subdirectories:

- [Separating Station](PLC-Programs/Separating-Station)
- [Storing Station](PLC-Programs/Storing-Station)

### Example PLC Program

```ladder
// Example Ladder Logic Program for Siemens S7-300
// Author: Your Name
// Date: YYYY-MM-DD

NETWORK
TITLE = "Start Button"
A  I0.0
AN M0.0
=  Q0.0
