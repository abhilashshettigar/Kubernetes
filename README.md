# Kubernetes
Learning Basic and Advance Stuff related to Kubernetes with every comment and Readme 

### Mac OS
```sh
install hyperhit and minikube
brew update
brew install hyperkit
brew install minikube
kubectl
minikube
```

### Windows OS 
>! Need to install choco. Follow this steps for installation using this [link:-](https://medium.com/@JockDaRock/installing-the-chocolatey-package-manager-for-windows-3b1bdd0dbb49)
```sh
minikube start --vm-driver hyperv   
```
you can also use minikube start without specifying any vm driver 

```sh
kubectl                             
minikube
```


#### Generic Commands
| Commands                                                  | Description                                           |
| --------------------------------------------------------- | ----------------------------------------------------- |

| minikube status                                            |  shows details related to minikube                      |                           
| kubectl version                                            |  shows details regarding server and client version      |                    
| kubectl get nodes                                          | shows how many nodes are there                          |
| kubectl get pod                                            |  shows number of pods active                            |
| kubectl get services                                       |  shows number of services                               |    
| kubectl create deployment nginx-deployment --image=nginx   | creates deployment with given image                     |     
| kubectl get deployment                                     | shows list of deployments                               |
| kubectl get replicaset                                     | shows list of replicaset created while deployment       |                   
| kubectl edit deployment nginx-deployment                   | can edit config for deployment using cmd                |          
| kubectl kubectl describe pod nginx-deployment              | shows events regarding pod                              |
| kubectl logs nginx-deployment --[pod name]                 | shows logs for pods for that deployment                 |         
| kubectl exec -it [pod name] -- /bin/bash                   | used for interactivity inside container                 |         
| kubectl delete deployment nginx-deployment                 | used for deleting deployment                            |
| kubectl get all                                            | getting all kubectl components                          |
| kubectl get pod/deployment/service --watch                 | continues watch while components are created            |              
| kubectl get pod -o wide                                    | gives extra details regarding pods                      |    
| kubectl apply -f [filename] / nginx-deployment.yaml        | create any stack using yaml file                        |  
| kubectl delete -f [filename] / nginx-deployment.yaml       | deletes any stack using yaml file                       |   
| minikube service [service name]                            | gives external ip for service [step need in local setup]|                          


### Important Points
- configMap and secret files must be created before deployment are created