# Node.js Dev Container

`Node.js`開発用 Docker コンテナ

## Usage

`$ git clone https://github.com/miolab/node_docker.git`

`$ cd node_docker`

`$ docker-compose up -d`

## Execution Example

実行例（`src/sample_hello.js`）

```
$ docker-compose run --rm app node sample_hello.js
Hello, node docker!
```

## Environment

- Node.js

  ```
  $ docker-compose logs -f
  Attaching to node_container
  node_container | Welcome to Node.js v12.16.1.
  ```

- npm

  ```
  $ docker-compose run --rm app npm --version
  6.13.4
  ```

- Docker

  ```
  $ docker --version
  Docker version 19.03.8, ...

  $ docker-compose --version
  docker-compose version 1.25.4, ...
  ```
