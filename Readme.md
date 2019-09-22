# Docker image with [Dynomite](https://github.com/Netflix/dynomite/)

The image is on Dockerhub as [johnvmt/dynomite](https://hub.docker.com/r/johnvmt/dynomite)

You must include a configuration file at /dynomite/config/dynomite.yaml in the container

``$ docker run -d -p 8101:8101 -p 8102:8102 --name mydatabase -v /host/directory/dynomite.yaml:/dynomite/config/dynomite.yaml johnvmt/dynomite``
 
For configuration and architecture options, see the [Dynomite project](https://github.com/Netflix/dynomite/) documentation

See also: [docker-dynomite-redis](https://github.com/johnvmt/docker-dynomite-redis), which includes Redis