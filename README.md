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
   Edit the `.env` file to configure your environment settings for `MSSQL_SA_PASSWORD`. The password must be at least 8 characters long and contain characters from three of the following four sets: Uppercase letters, Lowercase letters, Base 10 digits, and Symbols..

3. Start the docker service:
   ```bash
   docker compose up -d
   ```

4. Install [Azure Data Studio](https://learn.microsoft.com/en-us/azure-data-studio/download-azure-data-studio?view=sql-server-ver16&tabs=win-install%2Cwin-user-install%2Credhat-install%2Cwindows-uninstall%2Credhat-uninstall) (mssql client):

4. Connect to the mssql server using Azure Data Studio. Use the following credentials:

- Server: localhost
- Authentication Type: SQL Login
- User name: SA
- Password: value of MSSQL_SA_PASSWORD in .env
- Check on `Remember password`
- Trust server certificate: True


## License

See the [LICENSE](LICENSE) file for details.
