# ENGO551_Lab5

For Lab 5, we created a MQTT javascript client with WebSockets and using the Paho library to handle MQTT messages in our web browser.

We used the MQTTX software as our client software, to test the functionailty of our browser to subscribe to a host and topic, and then publishing a message.

We also used the Geolocation API to send real-time location to the MQTT broker, and allow subscribers to receive the location in real time.

The user is able to determine the MQTT message broker and port. The user can start and end the connection with the broker. In case of disconnection, the user recieves
a message and the web browser automatically re-establishes the connection.

The user is able to publish any messages to any topics they choose, required they first subscribe to that topic.

There is a "share my status" button that generates a GeoJSON message that includes the users current temperature and a random value for the temperature. 
This message is also published to the MQTT topic.
A map is displayed and when "share my status" button is used, a marker is placed on the map at the users current location. When they click the marker, they can see
the current temperature value. The colour of the marker changes betwene green, blue and red depending on the current temperature value.
