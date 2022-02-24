# node-react-helm
Deploy Node and React application with the help of helm charts in K8s

## Steps to deploy using helm charts:

1. Deploy a minikube cluster with the help of below documentation.
   ```
   https://minikube.sigs.k8s.io/docs/start/
   ```
2. Once you install and start Minikube cluster, Please enable ingress addons in it. (If you're using any cloudprovider k8s service, make sure ingress controller and tiller is installed.)
```
   $ minikube addons enable ingress
```
3. Install the helm and kubectl clients in your system using below documentations:
```   
   Kubectl >> https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/
   helm >> https://helm.sh/docs/intro/install/ (If you're installing helm V3, you do not have to install and enable tiller in your cluster).
```

5. Clone this repository

```
git clone https://github.com/princeswarnkar/helm-demo.git

```

6. Please nevigate to respective directries to deploy the react and node application:

```
cd ./helm-demo/nodejs
cd ./helm-demo/reactjs

```
## Images Used

```
For React app >> princeox/reactjs-heml:latest
For Node App >> princeox/nodejs-heml:latest
```

## Note:

This Task has been configured and tested on Kubernetes version v1.20.0
