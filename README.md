# MSSQL with Docker

This repository contains a Docker-based MSSQL server setup.

## Prerequisites

- Git
- Docker and Docker Compose
- VSCode (optional)

## Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/michaeltansg/mssql-docker.git
   cd mssql-docker
   ```

2. Set up environment variables:
   ```bash
   cp .env.example .env
   ```
   Edit the `.env` file to configure your environment settings, especially the `MSSQL_SA_PASSWORD`.

3. Start the docker service:
   ```bash
   docker compose up -d
   ```


## License

See the [LICENSE](LICENSE) file for details.
