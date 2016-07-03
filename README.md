# Dockerised Rails Application

## Getting started

Building the image

```bash
git clone https://github.com/DataMinerUK/moby-dock-rails.git
cd moby-dock-rails
docker-compose build mobydock
docker-compose run --user "$(id -u):$(id -g)" mobydock rake db:reset # This builds the database
docker-compose up
```

Once the image has been built all you need to do to run the app is

```bash
docker-compose up
```

Running the app

```bash
docker-machine ip
```

In a browser go to the [ip of docker machine]:8000. Feed Moby Dock!
