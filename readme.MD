# How to Run Postgres and PGAdmin with Docker-Compose

This project allow run Postgres DB and PGAdmin without installing them.

Create .env file for env variables.

## Postgres Service

_**Add to you .env file**_

- `POSTGRES_USER=`
- `POSTGRES_PASSWORD=`
- `POSTGRES_DB=`
- `POSTGRES_PC_PORT=`

## PGAdmin Service

_**Add to you .env file**_
- `PGADMIN_DEFAULT_EMAIL= email-login-pg`
- `PGADMIN_DEFAULT_PASSWORD= pass-login-pg`
- `PGADMIN_PC_PORT= port-run-pg`

## PGAdmin Create Connection

- **General**:
  - _name: connection-name_
- **Connection**:
  - _host: docker-postgres-service-name_
  - _port: 5432_
  - _user: env-postgres-user_
  - _password: env-postgres-password_

## How to run

- **Start service**: in a terminal write `docker-compose up`
- **Stop service**: in a terminal write `docker-compose down`
