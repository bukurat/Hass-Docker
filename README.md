# Hass-Docker

Docker compose file for Home Assistant containers

This is a docker container stack for Home Assistant and related apps. Where possible, containers are on an internal docker network.

The .env files are the environment details that usually live under the ENVIRONMENT: tag.

Format for mapping volumes:
- /home/$USER/hass_config:/config
-    mapped to           : mapped from (in container)

The /config directory in the container is mapped to hass_config in my linux home directory.

Initial setup:
sudo apt-get update
sudo apt install docker.io
sudo systemctl start docker
sudo systemctl enable docker

Check Installed version:
docker --version

See https://linuxize.com/post/how-to-install-and-use-docker-on-ubuntu-20-04/
to install latest version from docker.com. This is usually more up to date than the one in the Ubuntu repository.

See https://docs.docker.com/engine/install/linux-postinstall/
to manage docker as a non root user.

See https://docs.docker.com/compose/install/ to install docker-compose. Required for my script.

