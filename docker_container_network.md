# Create network

## 1- Network status
	
	```
	docker network ls
	```
	```
	docker network inspect
	```

## 2- Create docker network
	
	docker network create --subnet=IP_RANG --driver=DRIVER name

## 3- Run docker container

	docker run -d --name container_name --network=network_name container/... 

