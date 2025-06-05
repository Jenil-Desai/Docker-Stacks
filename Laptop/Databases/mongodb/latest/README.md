Docker-Stacks/Laptop/Databases/mongodb/latest/README.md
# MongoDB (latest) - Docker Stack

This directory contains the Docker Compose configuration for running the **latest version** of MongoDB in a containerized environment.

## Overview

- **Service:** MongoDB
- **Version:** latest
- **Category:** Databases
- **Environment:** Laptop

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/) installed on your machine
- [Docker Compose](https://docs.docker.com/compose/install/) (if not included with Docker Desktop)
- Sufficient system resources (at least 2 CPU cores, 2GB RAM recommended)

## Files

- `docker-compose.yaml` – Main Docker Compose configuration for MongoDB
- `.env.example` – Example environment variables file (copy to `.env` and modify as needed)
- `.env` – Your environment-specific variables (should not be committed)

## Usage

### 1. Clone the Repository

```sh
git clone https://github.com/Jenil-Desai/Docker-Stacks.git
cd Docker-Stacks/Laptop/Databases/mongodb/latest
```

**Or download just the `docker-compose.yaml` using `curl`:**

```sh
curl -o docker-compose.yaml https://raw.githubusercontent.com/Jenil-Desai/Docker-Stacks/main/Laptop/Databases/mongodb/latest/docker-compose.yaml
```

### 2. Configure Environment Variables

Copy the example environment file and edit as needed:

```sh
cp .env.example .env
# Edit .env to set your MongoDB root password and other settings
```

### 3. Start the MongoDB Container

```sh
docker compose up -d
```

This will pull the MongoDB image (if not already present) and start the container in detached mode.

### 4. Accessing the Database

- **Port:** The default port is usually `27017` (check your `.env` and `docker-compose.yaml`).
- **Username/Password:** As set in your `.env` file.
- **Connection String:** Refer to the output of `docker compose ps` or your `.env` settings.

You can connect using MongoDB Compass, the `mongo` shell, or any compatible client.

### 5. Stopping the Service

```sh
docker compose down
```

## Notes

- The first startup may take a minute as the database is initialized.
- Data persistence depends on the volume configuration in `docker-compose.yaml`.
- For advanced configuration, refer to the official MongoDB Docker image documentation.

## Troubleshooting

- Check logs with `docker compose logs -f`.
- Ensure your system meets the minimum resource requirements.
- If you encounter port conflicts, adjust the port mapping in `docker-compose.yaml`.

## References

- [MongoDB Docker Images](https://hub.docker.com/_/mongo)
- [Official MongoDB Documentation](https://docs.mongodb.com/)

---
**Maintained by:** Jenil Desai  
For issues or questions, please open an issue or contact [jenildev91@gmail.com](mailto:jenildev91@gmail.com).