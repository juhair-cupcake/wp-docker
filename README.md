# Docker-wp

This repo is for running WP in a `Docker Container`. I always `systemctl disable docker` because I don't wanna run docker 24/7. So for starting it I use `systemctl start docker` and `stop` for shut down.

## Run it

```
docker-compose up -d
```

- Wordpress on `localhost:8000`

## Change the ownership

```
# Get the folder because you wanna update the code and others...
sudo chown -R $USER:www-data wp-docker

# Give the folder back because you wanna install X from wp site...
sudo chown -R www-data:$USER wp-docker
```
