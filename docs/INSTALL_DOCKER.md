# Installing Docker + Docker Compose (Ubuntu)

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install -y docker.io
sudo systemctl enable --now docker
sudo apt install -y docker-compose-plugin
docker --version
docker compose version
