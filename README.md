# Full-Cycle First Project

This is a monorepo containing a project developed during the Full-Cycle Developer Program. The repository includes:

- `web-app`: Aplicação front-end desenvolvida em Angular v16.
- `user-service`: Back-end microservice built in nestJs.
- Docker Compose configuration to facilitate the execution of services.

Explore individual directories for more information about each component of the project.

root/
├── docker-compose.yml
├── README.md
├── web-app/
│   ├── src/
│   │   ├── app/
│   │   │   ├── ...
│   │   │   ├── (source-code Angular)
│   │   ├── ...
│   ├── package.json
│   ├── angular.json
│   ├── Dockerfile
├── user-service/
│   ├── src/
│   │   ├── ...
│   │   ├── (source-code)
│   │   ├── ...
│   ├── package.json
│   ├── Dockerfile
└── ...