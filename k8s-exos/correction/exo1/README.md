# Kubernetes exo 1
- Placer vous dans le dossier exo1
- Construire l'image et l'envoyer sur le docker.hub 
- Remplacer **<docker_id/image:tag>** par vos propres données 
- Déployer dans votre cluster k8s (minikube)
- Tester une requête http sur l'ip du cluser + port du service

```
docker build . -t <docker_id/image:tag>
docker push <docker_id/image:tag>
kubectl apply -f exo1.yml
curl <ip_cluster>:31201/page1.html
```