# What is the kubernets service?
### Service serves as a stable static IP and DNS for the application, which gives us the option to communicate with the Pods.
### Containers(Pods) change all the time, they stop, start, get new IP, and the service is the solution for that.
### Service routes our requests to the correct Pods.
#

# Scaling BackEnd Depoloyment
## Q.Explain why the frontend is accessible but backend is not
### A.The frontend is accessible because it is the public entry point for users.
###   The backend is internal-only and is accessed by the frontend inside the cluster to handle application logic.
###   The frontend was exposed externally using:
>###  minikube service frontend 
###   Reference:
### [https://github.com/almogbcr/kube/tree/main/logs/minikube/minikube-front-service.txt](https://github.com/almogbcr/kube/tree/main/logs/minikube/minikube-front-service.txt)
#####
#####
#####
## Q.Change replicas using kubectl (Without editing YAML)
### A.We can change replica using kubectl with:
>### kubectl scale --replicas=2 deploymentname
### Proof: [kubectl get pods](https://github.com/almogbcr/kube/blob/main/replica/scalebackend.log)


