# Repo for managing files for kubernetes
# Useful Commands

# Creating image and upload it to GCR
docker build -t <image_name> <directory>
docker tag <app_name> gcr.io/tag-name>
docker push <image-name-with-tag>

# Connecting to continer and creating pods, deployment
  
gcloud container clusters get-credentials <cluster-name> --zone=<zone-name>

kubectl apply -f <YAML file>
  
kubectl get pods
  
kubectl port-forward nginx 8080:80
  
kubectl delete -f <YAML file>
  
kubectl exec --it <POD name> -c <container name> --/bin/bash
  
kubectl describe deployments <deployment-name>
