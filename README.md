# PostgresQL using Docker

This docker-compose.yaml file will set up a PostgresQL image in a docker container.
This method is much more convenient than manually setting up a new Postgres database.
The image is based on Postgres 15 and Alpine 3.
Alpine is very popular for Docker containers because of its incredibly small size.

## Usage

1. Install Docker and docker-compose if you haven't already. The easiest way to do that is with [Docker Desktop](https://docs.docker.com/desktop/).
2. Download the `docker-compose.yaml` file or clone this repo.
3. Create a `.env` file in the same directory as the docker-compose.yaml. You can use the provided `.env.example` as a template.
4. Add `.env` to your gitignore. Information to log into the database SHOULD NOT be version controlled.
5. Open a terminal in the same directory as the docker-compose.yaml and run `docker-compose up -d` to run the container in the background. The database should be running at the port specified in `services.db.ports`.
