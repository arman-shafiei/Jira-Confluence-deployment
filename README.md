# Jira-Confluence-deployment

<p align="center" style="margin-bottom: 0px !important;">
  <img width="500" src="https://raw.githubusercontent.com/arman-shafiei/page/main/Logos/jira_confluence_docker.png" alt="Jira & Confluence & Docker Logo" align="center">
</p>

A docker compose template which you can use to deploy Jira and Confluence.

Via this deployment you can deploy Jira+Confluence with postgres database and nginx as a webserver.

The file structure is as follows:

- **Dockerfile**: Contains Dockerfiles for Jira and Confluence we're going to deploy.
- **nginx**: Contains nginx webserver config files.
- **server_config**: Config files to specify network settings for Jira & Confluence.
- **.env.example**: Consists of environment variables to be used for database, etc.
- **docker-compose.yml**: Main docker compose file to deploy our services.

## Compatibility

This deployment has been done and tested with:

- Postgres 11
- JDK 11
- Jira 8.21.0
- Confluence 7.15.0

## Deployment

Simply run:
```bash
docker-compose up -d
```