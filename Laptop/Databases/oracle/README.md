# Oracle Database Service

This directory contains Docker configurations and resources for running Oracle Database as a service within the `Databases` category for the `Laptop` environment.

## Structure

- **latest/**: Contains the latest supported Oracle Database Docker stack.
- **xe-11g/**: Contains the Oracle XE 11g Docker stack.

## Usage

1. Choose the desired version directory (e.g., `latest` or `xe-11g`).
2. Follow the instructions in the version-specific `README.md` or `docker-compose.yaml` to set up and run the Oracle Database container.

## Features

- Pre-configured Docker Compose files for easy setup.
- Example environment files for customization.
- Suitable for local development and testing.

## Prerequisites

- [Docker](https://www.docker.com/get-started) and [Docker Compose](https://docs.docker.com/compose/) installed on your laptop.
- Sufficient system resources to run Oracle Database containers.

## Getting Started

1. Navigate to the desired version directory:
   ```sh
   cd latest
   # or
   cd xe-11g
   ```
2. Copy the example environment file and adjust as needed:
   ```sh
   cp .env.example .env
   ```
3. Start the Oracle Database container:
   ```sh
   docker-compose up -d
   ```

## Notes

- Default credentials and ports can be configured in the `.env` file.
- For advanced configuration, refer to the official Oracle Database Docker documentation.

## Support

For issues or questions, please refer to the main repository's contact information or open an issue.

---