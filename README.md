# fibercleanall

REST API Fiber boilerplate

## ⭐️ Features

- REST API oriented
- Book CRUD example
- middleware
  - compress
  - CORS
  - ETag
  - recover
  - helmet
  - logger (optional)
  - limiter (optional)
- Environment config with .env
- JSON Error handling
- GORM V2
- Docker
- Live reloading (Air or Fresh)
- Testing

## ⚙️ Usage

You can fork this repo or use [fibercleanall as a package](https://github.com/embedmode/fibercleanall/blob/main/main.go)

- git clone https://github.com/embedmode/fibercleanall.git
- Copy .env.example to .env
- Install postgres or use docker-compose up postgres
- go mod download
- go run .
- Go to localhost:8080

## 🚧 Development

> Check .env file for database variables

```sh
# Install postgres or use docker-compose
docker-compose up postgres
go test ./...
air
# or fresh
```

## 🐳 Docker

```sh
# postgres + server
docker-compose up

# Building and running docker image (you will need postgres)
docker build -t fibercleanall .
docker run -d -p 8080:8080 fibercleanall

# only postgres
docker-compose up postgres
```

## 📜 Changelog

We use [GitHub releases](https://github.com/embedmode/fibercleanall/releases).

## 🔐 Security

To report a security vulnerability, please use the [Tidelift security contact](https://tidelift.com/security).

## 📄 License

This project is licensed under the terms of the
[MIT license](/LICENSE).
