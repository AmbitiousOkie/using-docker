Using Docker
=====

Using Docker on MacOS X.

## Install Docker

Docker must run inside a linux virtual machine. Be sure you have installed VirtualBox:

[virtualbox.org](https://www.virtualbox.org/)

Install docker with the official docker package:

[docker.com/installation](https://docs.docker.com/installation/)

Or install via homebrew:

```
brew install boot2docker
```

## Initialize Docker

Run `boot2docker init` at the command line once to initialize a VM for docker. Then at the command line run:

```
boot2docker start
$(boot2docker shellinit)
```

Add docker to launchctl to have it automatically start when you log in.

## Official Docker Images

Node

[https://registry.hub.docker.com/_/node/](https://registry.hub.docker.com/_/node/)

MongoDB

[https://registry.hub.docker.com/_/mongo/](https://registry.hub.docker.com/_/mongo/)

Redis

[https://registry.hub.docker.com/_/redis/](https://registry.hub.docker.com/_/redis/)

Nginx

[https://registry.hub.docker.com/_/nginx/](https://registry.hub.docker.com/_/nginx/)

Rails

[https://registry.hub.docker.com/_/rails/](https://registry.hub.docker.com/_/rails/)

## Additional References

Command Line Reference

[http://docs.docker.com/reference/commandline/cli/](http://docs.docker.com/reference/commandline/cli/)

Dockerfile Reference

[https://docs.docker.com/reference/builder/](https://docs.docker.com/reference/builder/)

Docker-Compose Reference

[https://docs.docker.com/compose/yml/](https://docs.docker.com/compose/yml/)

