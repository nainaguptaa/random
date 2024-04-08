# Steps to run 


First, Open this up this assignment on github codespace

Then run the following commands to start up:

1. minikube start
2. minikube addons enable ingress


To run the nginx files:
1. kubectl apply -f nginx-dep.yaml
2. kubectl apply -f nginx-svc.yaml
3. kubectl apply -f nginx-ingress.yaml
4. kubectl apply -f nginx-configmap.yaml


To run app-1 files:
1. kubectl apply -f app-1-dep.yaml
2. kubectl apply -f app-1-svc.yaml
3. kubectl apply -f app-1-ingress.yaml


To run app-2 files:
1. kubectl apply -f app-2-dep.yaml
2. kubectl apply -f app-2-svc.yaml
3. kubectl apply -f app-2-ingress.yaml


Then finally, run these commmands to see everyhthing working (run these multiple times to see both app 1 and app 2 Hello world message):
1. curl http://$(minikube ip)
2. curl http://$(minikube ip)/app


## Screenshots of output







