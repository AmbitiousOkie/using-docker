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

Install docker-compose via homebrew:

```
brew install docker-compose
```

## Initialize Docker

Run `boot2docker init` at the command line once to initialize a VM for docker. Then at the command line run:

```
boot2docker start
$(boot2docker shellinit)
```

Add docker to launchctl to have it automatically start when you log in.

## Using Docker-Compose

```
docker-compose build
docker-compose up
```

In development you must use the IP address from your docker VM to view application running in containers. Get the IP address:

```
boot2docker ip
```

## Interact with a container

Interact with a running container using `docker exec`:

```
docker exec -it [container-id] bash
```

## Official Docker Images

<table>
	<tr>
		<td> Node </td>
		<td> <a href="https://registry.hub.docker.com/_/node/">https://registry.hub.docker.com/_/node/ </a>
		</td>
	</tr>
	<tr>
		<td> MongoDB </td>
		<td> <a href="https://registry.hub.docker.com/_/mongo/">https://registry.hub.docker.com/_/mongo/ </a>
		</td>
	</tr>
	<tr>
		<td> Redis </td>
		<td> <a href="https://registry.hub.docker.com/_/redis/">https://registry.hub.docker.com/_/redis/ </a>
		</td>
	</tr>
	<tr>
		<td> Nginx </td>
		<td> <a href="https://registry.hub.docker.com/_/nginx/">https://registry.hub.docker.com/_/nginx/ </a>
		</td>
	</tr>
	<tr>
		<td> Rails </td>
		<td> <a href="https://registry.hub.docker.com/_/rails/">https://registry.hub.docker.com/_/rails/ </a>
		</td>
	</tr>
</table>

## Official References

Command Line Reference

[http://docs.docker.com/reference/commandline/cli/](http://docs.docker.com/reference/commandline/cli/)

Dockerfile Reference

[https://docs.docker.com/reference/builder/](https://docs.docker.com/reference/builder/)

Docker-Compose Reference

[https://docs.docker.com/compose/yml/](https://docs.docker.com/compose/yml/)

Managing Data in Containers

[https://docs.docker.com/userguide/dockervolumes/](https://docs.docker.com/userguide/dockervolumes/)

## Tutorials and Other Links

A sample Docker workflow with Nginx, Node.js and Redis

[http://anandmanisankar.com/posts/docker-container-nginx-node-redis-example/](http://anandmanisankar.com/posts/docker-container-nginx-node-redis-example/)

Node with Docker - Continuous Integration and Delivery

[http://mherman.org/blog/2015/03/06/node-with-docker-continuous-integration-and-delivery/](http://mherman.org/blog/2015/03/06/node-with-docker-continuous-integration-and-delivery/)