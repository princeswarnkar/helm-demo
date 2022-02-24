
## Docker image build commands
```
docker build -t ${IMAGE_NAME}:${IMAGE_TAG} .
```

## Deploy on Kubernetes Using Helm

Prerequisites:

- Kubernetes Cluster 1.20.0 (MiniKube or any other provider).
- Helm and Kubectl

Run below commands to deploy the applicaton on K8s using helm
```
$ helm install node nodejs-helm/
```
Note: If you're using Minikube, Please make an entry of your minikube IP in /etc/hosts file as below:
```
$ kubectl get ingress -o wide  #get the IP of your minikube node

$(minikube_node_ip)   nodejs.example.com
```
