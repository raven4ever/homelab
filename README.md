# Homelab Setup

## Setup

```shell
sudo mkdir -p /data/{container_data, downloads, media}
sudo chown -R $USER:$USER /data
mkdir -p /data/media/{movies, series}
mkdir -p /data/downloads/{incomplete, radarr, sonarr}

sudo cp portainer.service /etc/systemd/system/
sudo systemctl daemon-reload
sudo systemctl enable portainer.service
sudo systemctl start portainer.service
```
