## Development

Install all the required packages/dependencies using yarn

### `yarn`

Serve the app to browser

### `yarn start`

## Checklist

- [x] Use localstorage to store todos
- [ ] Improve app responsiveness on all devices

## Docker image build Commands

docker build -t {IMAGE_NAME}:${IMAGE_TAG} .


## Deploy on Kubernetes

Prerequisites:

- Kubernetes Cluster (MiniKube or any other provider).
- Helm and Kubectl

Run below commands to deploy the applicaton on K8s using helm

helm install react reactjs-helm/

Note: If you're using Minikube, Please make an entry of your minikube IP in /etc/hosts file as below:

(minikube_ip)   react.example.com

