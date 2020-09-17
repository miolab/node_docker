# Node.js Dev Container

`Node.js` の Docker 開発用リポジトリ

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
  node_container | Welcome to Node.js v14.10.1.
    .
    .
  ```

- npm

  ```
  $ docker-compose run --rm app npm --version
  6.13.8
  ```

- Docker

  ```
  $ docker --version
  Docker version 19.03.12, ...

  $ docker-compose --version
  docker-compose version 1.26.2, ...
  ```
