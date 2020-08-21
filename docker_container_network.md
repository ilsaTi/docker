# Create network

## 1- Network status

You can start by listing the the network with the following command:
```
docker network ls
```

Notice the driver. Let's use  `bridge` as driver in the next steps. Inspect it with `docker network inspect` command as follow:


```
docker network inspect bridge
```

## 2- Create docker network
	
	docker network create --subnet=IP_RANG --driver=DRIVER name

## 3- Create docker container

Use `docker run --network=` to create a container. 


With [hello-world](https://hub.docker.com/_/hello-world) image, the command is as follow: 
```
docker run -it --name network=newNetwork containerHello hello-world
```

