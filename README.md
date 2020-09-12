# ble-mqtt-bridge
A Python Bluetooth LE to MQTT bridge

## Install device dependencies (you only need to do this once each device)
```
sudo apt install libglib2.0-dev virtualenv
```

## Clone this repository
Navigate to add-on application folder
```
cd /opt
```
Clone repository
```
sudo clone https://github.com/aidan-parkinson/ble-mqtt-bridge.git
```

## Create virtual environment and install project dependencies
Navigate to project folder
```
cd /opt/ble-mqtt-bridge
```
Create a virtual environment
```
sudo virtualenv venv
```
Install project dependencies
```
sudo pip3 install bluepy paho-mqtt
```

## Run the bridge
Run like this:
```
sudo source /opt/ble-mqtt/bin/activate

sudo /opt/ble-mqtt/ble-mqtt-bridge.py
```
