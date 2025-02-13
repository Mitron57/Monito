# Monito
Web service with container status dashboard

# Features
 - Scans host for Docker containers
 - Pings them and saves results in PostgreSQL database
 - Results can be accessed via frontend, which automatically polls backend

# Launch
If you want just run locally and don't care about anything just clone this repository and do this:
 - Create .env files in submodules (see [DockMon.example](https://github.com/Mitron57/DockMon/blob/main/.env.example), [Frontend.example](https://github.com/Mitron57/MonitoFrontend/blob/main/.env.example)), or simply rename them without .example and run
```shell
docker-compose up -d --build
```
So, if you want to tune service with your preferences, do these steps:

- Open [docker-compose.yaml](docker-compose.yaml) and manually specify all you want according to manual for PostgreSQL docker image
- Specify env files and configs for services (see [DockMon](https://github.com/Mitron57/DockMon), [Pinger](https://github.com/Mitron57/Pinger), [Frontend](https://github.com/Mitron57/MonitoFrontend))

...and then run command above

Enjoy!
