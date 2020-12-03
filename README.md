# DAVE

```
wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop/config
export KUBECONFIG=config
kubectl config view
kubectl get namespaces

wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop/dave/namespace.yaml
cat namespace.yaml
kubectl apply -f namespace.yaml
kubectl get namespace dave
kubectl get namespace dave -o yaml 
kubectl describe namespace dave
kubectl apply -f namespace.yaml


wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop/dave/deployment.yaml
cat deployment.yaml
kubectl apply -f deployment.yaml
kubectl get nginx-deployment -n dave
kubectl get nginx-deployment -n dave -o yaml 
kubectl describe nginx-deployment -n dave
kubectl apply -f deployment.yaml

wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop/dave/service.yaml
cat service.yaml
kubectl apply -f service.yaml
kubectl get nginx-service -n dave
kubectl get nginx-service -n dave -o yaml 
kubectl describe nginx-service -n dave
kubectl apply -f service.yaml
```

# TONY

```
wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop/config
export KUBECONFIG=config
kubectl config view
kubectl get namespaces

wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop/tony/namespace.yaml
cat namespace.yaml
kubectl apply -f namespace.yaml
kubectl get namespace tony
kubectl get namespace tony -o yaml 
kubectl describe namespace tony
kubectl apply -f namespace.yaml


wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop/tony/deployment.yaml
cat deployment.yaml
kubectl apply -f deployment.yaml
kubectl get nginx-deployment -n tony
kubectl get nginx-deployment -n tony -o yaml 
kubectl describe nginx-deployment -n tony
kubectl apply -f deployment.yaml

wget https://raw.githubusercontent.com/green-redcloud3/kubernetes/main/workshop/tony/service.yaml
cat service.yaml
kubectl apply -f service.yaml
kubectl get nginx-service -n tony
kubectl get nginx-service -n tony -o yaml 
kubectl describe nginx-service -n tony
kubectl apply -f service.yaml
```