# Arduino_Flask
Link thingspeak = https://thingspeak.com/channels/1350261

# Run json server for receice of board 
json-server --watch data.json -H 172.20.10.12 -p 3000

# Run main.py

# must rub server MQTT first by
mqtt % mosquitto -c mosquitto.conf -v

# For Check valur from sensor
mosquitto_sub -i node_01 -h 172.20.10.12 -t "led or dht11"

