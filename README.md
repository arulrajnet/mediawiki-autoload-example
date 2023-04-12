Mediawiki Auto Initialization base data
------------------------------------------

This will create a docker container with mediawiki and mysql database. This will load the admin user and the default page with the content from the file `./data/mediawiki/LocalSettings.php`.

## Prerequisites

* [Docker](https://www.docker.com/)
* [Docker Compose](https://docs.docker.com/compose/)

## Installation

### Docker

```
curl -sSL https://get.docker.com/ | sh
sudo usermod -aG docker ${USER}
```

### Docker Compose

```
sudo curl -sSL https://github.com/docker/compose/releases/download/v2.17.2/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

## Bringup mediawiki

```
docker-compose up -d
```

To access the mediawiki, go to http://localhost:8080

Credential to login : admin / Welcome@123
