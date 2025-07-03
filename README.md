# Aquaponics System Monitoring

This project contains Node-RED flows designed to monitor key parameters of an aquaponics system.

## Features:

* **Temperature Monitoring**:
    * Reads water temperature data.
    * Displays real-time temperature on a dashboard gauge and a historical chart.
    * Sends a WhatsApp alert if the temperature exceeds 25°C.
      <img src= "https://github.com/GloryBinkatabana/NodeRed/blob/c2db0674154890148e22836abfa6168aa2ce4dba/tempsensor.png">

* **TDS (Total Dissolved Solids) Monitoring**:
    * Measures TDS levels in the water.
    * Visualizes TDS data on a dashboard gauge and a historical chart.
    * Triggers a WhatsApp alert if TDS levels are too high (above 1000 ppm).
      <img src= "https://github.com/GloryBinkatabana/NodeRed/blob/c2db0674154890148e22836abfa6168aa2ce4dba/TDSsensor.png">

* **Turbidity Monitoring**:
    * Detects water clarity by measuring turbidity.
    * Presents turbidity levels on a dashboard gauge and a historical chart.
    * Dispatches a WhatsApp alert if turbidity is too high (above 900 NTU).
      <img src= "https://github.com/GloryBinkatabana/NodeRed/blob/c2db0674154890148e22836abfa6168aa2ce4dba/Turbiditysensor.png">

## Technical Details:

* **Platform**: Node-RED
* **Communication**: MQTT broker (`b30de00f7f77044f`, named "Our server") for receiving sensor data.
* **Alerting**: Integrated with a WhatsApp messaging service for critical alerts.
* **Dashboard**: User interface accessible via the "Aquaponics system" UI tab, featuring a dark theme.
