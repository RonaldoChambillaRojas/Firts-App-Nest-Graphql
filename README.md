<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Docker - Bind Volumes - Ubuntu

```bash
docker run \
  --name nest-app \
  -d \
  -w /app \
  -p 3000:3000 \
  -v "$(pwd)":/app \
  node:18-alpine \
  sh -c "yarn install && yarn start:dev"
```
## Docker - Bind Volumes - Windows

```bash
docker run `
--name nest-app `
-w /app `
-p 3000:3000 `
-v C:\nombre\de\tu\ruta\actual:/app `
-e CHOKIDAR_USEPOLLING=true ` # Opcional
node:18-alpine3.21 `
sh -c "yarn install && yarn start:dev"
```