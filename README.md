# Simple WordPress setup with Docker

Pre-requisites:

Create .env file to root with following environment variables:
WORDPRESS_DB_PASSWORD=<random-password>
MYSQL_ROOT_PASSWORD=<same-random-password>
TZ=<optional-time-zone>

Update nginx/conf/wordpress.conf hostname with your own host.

## Setup

```
docker-compose up
```

Open browser at http://<hostname> and run the setup.

## Technical

Setup uses nginx as front-end, then WordPress container has Apache2 handling the actual site.
This way it's easy to stop traffic to the site by stopping the nginx service.

MariaDB acts as the database server.
All networking is happening inside Docker virtual network.

## TODO

Add HTTPS support with certbot.


Enjoy!
