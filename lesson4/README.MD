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
>###  "minikube service frontend" 
###   Reference:


