# Mediaserver

Deploying the stack will spin up two containers: plex and tautulli. 

Plex is a media server application. It has two mounted volumes:
* /config
* /library

Both of these will be put into your `/` within the container. The config directory holds all the configs for the application, as well as the metadata for your media. Depending on the size of your library the metadata can take up a significant amountspace, so it is advised to mount this on a somewhat larger partition.
The library directory can be used to create sub-directories for the various forms of media that plex handles (shows, movies, music, pictures, home videos).

Tautulli is a monitoring and telemetry application for plex. It collects various statistics as well as monitors activity, and can be used to send and receive notifications through third party platforms.
It only has a single mount point, `/config`, which will hold the applications configs.

Deploying this stack requires Docker and Docker-compose.

How to deploy:
```
docker-compose up -d
```