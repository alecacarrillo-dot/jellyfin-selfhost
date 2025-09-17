# jellyfin-selfhost

# Jellyfin Docker Setup – Self-Hosted Media Library

This repository contains a simple Docker Compose setup to run [Jellyfin](https://jellyfin.org/), a free media server.

---

## 1. Project Overview
Organize, stream, and share your media with Jellyfin. This setup uses host networking, persistent volumes, and optional custom fonts for subtitles.

---

## 2. Prerequisites
- Linux server (Ubuntu recommended)  
- Sufficient storage for your media  
- Docker + Docker Compose installed  
  - [See detailed installation instructions](docs/INSTALL_DOCKER.md) if needed

---

## 3. Setup Instructions
1. Clone this repository:  
   ```bash
   git clone https://github.com/<yourusername>/<yourrepo>.git
   cd <yourrepo>

2. Create required directories (Docker won’t create all subfolders automatically):
   
 ```bash
   mkdir -p config cache media/music fonts
