# Curriculum Vitae
Curriculum Vitae

## Requirements

Please make sure to fulfill all these requirements:

- [Install Docker](https://docs.docker.com/get-docker/)

## Set environment variables

From the *devops* directory copy the example Dotenv file:

```sh
cp .env.example .env
```

Update environment variables if needed.

| Variable                        | Description |
| ------------------------------- |-------------|
| `ENV`                           | Current environment (could be "local" or "production"); stay on `local` for development environment |
| `COMPOSE_PROJECT_NAME`          | Sets the project name. This value is prepended along with the service name to the container on start up. |
| `COMPOSE_CONVERT_WINDOWS_PATHS` | Enable path conversion from Windows-style to Unix-style in volume definitions. Users of Docker Machine on Windows should always set this. |
| `DOCKER_DATA`                   | Path of the repertory where to persist data on your host (like the database) |
| `DOCKER_HOST_IP`                | Docker host's gateway IP address (needed for the DNS config between the frontend and api containers) |

## Start the environment

From the *devops* directory start the environment:

```sh
./bin/start
```

## Generate the resume file

From the *devops* directory generate the pdf resume file:

```sh
./bin/resume/generate
```
