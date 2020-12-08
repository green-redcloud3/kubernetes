# START YOUR WORKSTATION

```
docker run --rm --name dip-workstation -it -v c:\PROJECTS\dip-docs\platform:/platform dip:latest bash
```

Once you are in your container set your aws credentials


# DAVE

```
wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop_1/config
export KUBECONFIG=config
kubectl config view
kubectl get namespaces

wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop_1/dave/namespace.yaml
cat namespace.yaml
kubectl apply -f namespace.yaml
kubectl get namespace dave
kubectl get namespace dave -o yaml 
kubectl describe namespace dave
kubectl apply -f namespace.yaml


wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop_1/dave/deployment.yaml
cat deployment.yaml
kubectl apply -f deployment.yaml
kubectl get deployment nginx-deployment -n dave
kubectl get deployment nginx-deployment -n dave -o yaml 
kubectl describe deployment nginx-deployment -n dave
kubectl apply -f deployment.yaml

wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop_1/dave/service.yaml
cat service.yaml
kubectl apply -f service.yaml
kubectl get service nginx-service -n dave
kubectl get service nginx-service -n dave -o yaml 
kubectl describe service nginx-service -n dave
kubectl apply -f service.yaml
```

# TONY

```
wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop_1/config
export KUBECONFIG=config
kubectl config view
kubectl get namespaces

wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop_1/tony/namespace.yaml
cat namespace.yaml
kubectl apply -f namespace.yaml
kubectl get namespace tony
kubectl get namespace tony -o yaml 
kubectl describe namespace tony
kubectl apply -f namespace.yaml


wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop_1/tony/deployment.yaml
cat deployment.yaml
kubectl apply -f deployment.yaml
kubectl get deployment nginx-deployment -n tony
kubectl get deployment nginx-deployment -n tony -o yaml 
kubectl describe deployment nginx-deployment -n tony
kubectl apply -f deployment.yaml

wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop_1/tony/service.yaml
cat service.yaml
kubectl apply -f service.yaml
kubectl get service nginx-service -n tony
kubectl get service nginx-service -n tony -o yaml 
kubectl describe nginx-service -n tony
kubectl apply -f service.yaml
```
