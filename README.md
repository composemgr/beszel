## 👋 Welcome to beszel 🚀

Beszel - Lightweight server monitoring platform

## 📋 Description

Beszel is a lightweight server monitoring platform with a web interface for tracking system metrics, uptime, and performance across multiple servers.

## 🚀 Services

- **server**: Beszel monitoring server (`henrygd/beszel:latest`)

## 📦 Installation

### Using curl
```shell
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/beszel/main/docker-compose.yaml" | docker compose -f - up -d
```

### Using git
```shell
git clone "https://github.com/composemgr/beszel" ~/.local/srv/docker/beszel
cd ~/.local/srv/docker/beszel
docker compose up -d
```

### Using composemgr
```shell
composemgr install beszel
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
BASE_HOST_NAME=${HOSTNAME}
```

## 🌐 Access

- **Web Interface**: http://172.17.0.1:60047

## 📂 Volumes

- `./rootfs/data/beszel` - Application data and metrics

## 🔍 Logging

```shell
docker compose logs -f server
```

## 🛠️ Management

```shell
docker compose up -d
docker compose down
docker compose pull && docker compose up -d
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
