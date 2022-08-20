# aks-nginx001
aks-nginx001.yaml

git clone https://github.com/ayhansevimli/aks-nginx001.git
cd aks-nginx001
kubectl apply -f aks-nginx001.yaml
kubectl expose deployment aks-nginx001-deployment --type=LoadBalancer --port=8000 --target-port=80 --name=aks-nginx001-service-port-8000
kubectl get deployment
kubectl get pod
kubectl get replicaset
kubectl get service
kubectl delete -f aks-nginx001.yaml
kubectl delete service aks-nginx001-service-port-8000
