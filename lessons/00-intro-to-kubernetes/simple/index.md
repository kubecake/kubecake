# From Docker to Kubernetes

## Build and test using Docker

See: https://bitpress.io/simple-approach-using-docker-with-php/

```
cd php7-apache
docker build --file docker/Dockerfile -t myphp .
docker run --rm -p 8080:80 myphp
# Visit http://localhost:8080/
```

## Upload image to Docker Hub registry

```
docker tag myphp <username>/myphp:latest
docker push <username>/myphp
```

## Create deployment to Kubernetes

```
kubectl apply -f deployment.yaml -f service.yaml
kubectl get pods
# Wait until ready
minikube addons enable ingress
kubectl get services
minikube service myphp-svc
```
