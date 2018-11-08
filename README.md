# MQTT micro-ticker #

### test run ###

Just run:
```
docker-compose up
```
### Config ###

See docker-compose.yml for examples.

User credentials for MQTT authentication are provided via JSON files. Mount
them to /run/secrets/mqtt_listener.json and /run/secrets/mqtt_publisher.json or
provide ENV variables MQTT_LISTENER_CREDENTIALS and MQTT_PUBLISHER_CREDENTIALS
to specify a custom location.

The two files have the following JSON structure (replace with your values):
```
{
    "username": "myusername",
    "password": "mypassword"
}
```
