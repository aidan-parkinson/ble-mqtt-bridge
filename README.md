# ble-mqtt-bridge
A Python Bluetooth LE to MQTT bridge

## Download the latest ca certificate to appropriate folder
```
cd /etc/ssl/certs
sudo rm learning-iot-ca.crt
sudo curl -0 https://learning-iot.aidanparkinson.xyz -o learning-iot-ca.crt
```

## Install device dependencies
```
sudo apt update
sudo apt-get install libglib2.0-dev virtualenv python3-pip
pip3 --version
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

## To run the bridge (start at this point if you have completed this process before on your device)
Navigate to project folder
```
cd /opt/ble-mqtt-bridge/
```
Activate the virtual evironment with pre-installed dependencies
```
source venv/bin/activate
```
Run the `ble-mqtt-bridge.py` controller
```
sudo python3 ble-mqtt-bridge.py
```
