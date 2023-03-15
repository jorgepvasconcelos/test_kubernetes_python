# test_kubernetes_python

# Create image

docker build -t <user>/fast-api-image .

docker push <user>/fast-api-image

docker run -p 8000:8000 fast-api-image

# start minikube
minikube start

# apply kubectl
kubectl apply -f kubernetes.yaml

minikube dashboard

minikube addons enable metrics-server
minikube addons enable portainer

# minikube commands
minikube service fast-api-service

# kubectl commands
kubectl get deployment
kubectl get service
