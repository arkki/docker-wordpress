# Simple WordPress setup with Docker

Pre-requisited:

Create .env file to root with following environment variables:
WORDPRESS_DB_PASSWORD=<random-password>
MYSQL_ROOT_PASSWORD=<same-random-password>
TZ=<optional-time-zone>

Update nginx/conf/wordpress.conf hostname with your own host.

Setup:
```
docker-compose up
```

Open browser at http://<hostname> and run the setup.

Enjoy!
