Here these are the deployment cum service and configmap and secret configuration files for practicing setup of a k8s cluster on minikube


Way to start to this cluster -
 - post cloning this repo, it is expected we have minikube installed on system. We start minikube by following command : "minikube start" (in terminal)
 - Once the miniikube starts our first task is to add the configmap and secret configuration files to the environment, using the folllowing commands:
	- kubectl apply -f mongo-config.yaml
	- kubectl apply -f mongo-secret.yaml
 - Once the configmap and secret file are added now we can add the deployment files, using the following commands:
	- kubectl apply -f mongo.yaml
	- kubectl apply -f webapp.yaml
 - Now once all the files are added, to check about status of the cluster use following command:
	- kubectl get all
