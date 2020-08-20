# Create network

## 1- Network status

You can start by listing the the network with the following command:
```
docker network ls
```

Notice the driver. Let's use  bridge as driver in the next steps.


```
docker network inspect bridge
```

## 2- Create docker network
	
	docker network create --subnet=IP_RANG --driver=DRIVER name

## 3- Run docker container

	docker run -d --name container_name --network=network_name container/... 

