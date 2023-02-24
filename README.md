# Playground for Telegraf, InfluxDB, Grafana (TIG) Stack

## ⚡️ Getting Started

Clone the project

```bash
git clone https://github.com/huntabyte/tig-stack.git
```

Navigate to the project directory

```bash
cd tig-stack
```

Copy the environment template file, `.env.template`,  `.env` file

```bash
cp .env.template .env
```

Update the environment variables used to setup and deploy the stack inside `.env`

```bash
├── telegraf/
├── .env         <---
├── .env.template
├── docker-compose.yml
├── entrypoint.sh
└── ...
```

Customize the `telegraf.conf` file which will be mounted to the container as a persistent volume

```bash
├── telegraf/
│   ├── telegraf.conf <---
├── .env
├── .env.template
├── docker-compose.yml
├── entrypoint.sh
└── ...
```

Start the services

```bash
docker-compose up -d
```

## Docker Images Used (Official & Verified)

[**Telegraf**](https://hub.docker.com/_/telegraf) / `1.19`

[**InfluxDB**](https://hub.docker.com/_/influxdb) / `2.1.1`

[**Grafana-OSS**](https://hub.docker.com/r/grafana/grafana-oss) / `8.4.3`

## Thanks

This project was forked from <https://github.com/huntabyte/tig-stack.git> and
modified to act as a playground for training.
