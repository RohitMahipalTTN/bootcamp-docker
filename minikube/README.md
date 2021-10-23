# bootcamp-docker

step 1:
kubectl create ns rohit

step 2:(https://medium.com/bb-tutorials-and-thoughts/how-to-use-own-local-doker-images-with-minikube-2c1ed0b0968)
eval $(minikube docker-env)

step 3:
docker build -t webserver_minikube .

step 4:
kubectl apply -f test_deployment.yaml 

step 5:
kubectl apply -f test_service.yaml         

step 6:
(https://www.bmc.com/blogs/kubernetes-configmap/)
