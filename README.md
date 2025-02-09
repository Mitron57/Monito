# Monito
Web service with container status dashboard

# Features
 - Scans host for Docker containers
 - Pings them and saves results in PostgreSQL database
 - Results can be accessed via frontend, which automatically polls backend

# Launch
If you want just run locally and don't care about anything just clone this repository, create .env files in submodules (see examples) and run
```shell
docker-compose up -d --build
```
So, if you want to tune service with your preferences, let's start

- Open [docker-compose.yaml](docker-compose.yaml) and manually specify all you want according to manual for PostgreSQL docker image
- Specify env files and configs for services (see [DockMon](./DockMon/README.md), [Pinger](./Pinger/README.md), [Frontend](./MonitoFrontend/README.md))

...and then run command above

Enjoy!
