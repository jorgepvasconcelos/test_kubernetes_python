# test_kubernetes_python

docker build -t fastapi-kubernetes .
docker run -p 8000:8000 fastapi-kubernetes
kubectl apply -f kubernetes.yaml

minikube dashboard