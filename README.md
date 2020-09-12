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
sudo git clone https://github.com/aidan-parkinson/ble-mqtt-bridge.git
```

## Create virtual environment and install project dependencies
Navigate to project folder
```
cd /opt/ble-mqtt-bridge/
```
Create a virtual environment
```
sudo virtualenv venv
```
Activate it
```
source venv/bin/activate
```
Install project dependencies
```
sudo pip3 install bluepy paho-mqtt
```
Deactivate the virtual environment
```
deactivate
```

## Run the bridge
Navigate to project folder
```
cd /opt/ble-mqtt-bridge/
```
Activate the virtual evironment with pre-installed dependencies
```
sudo source venv/bin/activate
```
Run the `ble-mqtt-bridge.py` controller
```
sudo python3 ble-mqtt-bridge.py
```
