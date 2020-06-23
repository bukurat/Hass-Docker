# Hass-Docker

Docker compose file for Home Assistant containers

This is a docker container stack for Home Assistant and related apps. Where possible, containers are on an internal docker network.

The .env files are the environment details that usually live under the ENVIRONMENT: tag.

Format for mapping volumes:
- /home/$USER/hass_config:/config
-    mapped to           : mapped from (in container)

The /config directory in the container is mapped to hass_config in my linux home directory.
