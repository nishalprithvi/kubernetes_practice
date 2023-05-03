Way to start to this cluster -
 - post cloning this repo, it is expected we have minikube installed on system. We start minikube by following command : "minikube start" (in terminal)
 - Once the minikube starts, now we can add the deployment files, using the following commands:
	- kubectl apply -f redis.yaml
	- kubectl apply -f web.yaml
 - Now once all the files are added, to check about status of the cluster use following command:
	- kubectl get all

