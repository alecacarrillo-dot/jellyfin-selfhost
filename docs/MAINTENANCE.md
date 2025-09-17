# Jellyfin Maintenance Guide

This guide contains information on accessing your Jellyfin server, updating the container, backing up configurations, and troubleshooting.

---

## 1. Accessing the Services
Once the container is running, you can access Jellyfin in your browser:


- **Same machine** → `http://localhost:8096`  
- **Another device on the network** → `http://HOSTIP:8096`  

The web interface will guide you through the initial setup, including creating an admin account and adding your media libraries.

---

## 2. Updates & Maintenance

### Updating Jellyfin
To update Jellyfin to the latest version:

docker compose pull
docker compose up -d

### Stopping and Starting Jellyfin

docker compose down
docker compose up -d

### Viewing Logs

docker compose logs -f

---

## 3. Troubleshooting

If media doesn’t appear in Jellyfin, check that the Docker user has read permissions for the media directories.
If another service is using port 8096, change the port in docker-compose.yml.
Check logs with docker compose logs -f if the container fails to start or behaves unexpectedly.
