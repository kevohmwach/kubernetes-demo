#Start cluster
minikube start

#Check running services
minikube status

#Pause Kubernetes without impacting deployed applications
minikube pause

#unpause minikube
minikube pause

#Halt the cluster
minikube stop

#Change the default memory limit (requires a restart):
minikube config set memory 9001

#Browse the catalog of easily installed Kubernetes services:
minikube addons list

#Create a second cluster running an older Kubernetes release:
minikube start -p aged --kubernetes-version=v1.16.1

#Delete all of the minikube clusters:
minikube delete --all

#***********************************************Kubectl***************************************
#create deployment
kubectl create deployment mongodb --image=mongo

#view created deployment
kubectl get deployment
kubectl get pod

#see pod logs in creation
kubectl describe pod mongodb-6cbc8c86c7-s9927

#Delete deployment/pod
kubectl delete deployment mongodb


