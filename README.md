helm create template helm-charts
helm template test .\helm-charts\


minikube start --ports=30100:30100
helm install god-release helm-charts
kubectl get pods -o wide