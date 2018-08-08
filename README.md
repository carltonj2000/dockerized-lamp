# LAMP in Docker

The code in this repository is based on the
[How to create a docker-based LAMP stack using docker-compose on Ubuntu 18.04 Bionic Beaver Linux](https://linuxconfig.org/how-to-create-a-docker-based-lamp-stack-using-docker-compose-on-ubuntu-18-04-bionic-beaver-linux)
artcile.

Use `docker-compose` to start the containers.

### Connect to mysql

```
docker exec -it <container-name> bash
# initialize the db with
mysql -u testuser --password=testpassword testdb < db.sql
# repl
mysql -u testuser --password=testpassword testdb
```
