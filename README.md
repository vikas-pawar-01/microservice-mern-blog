# microservice-mern-blog

### Run Project
- skaffold dev

### Build container pod
- docker build -t vpawar01/posts .

### Push docker build
- docker push vpawar01/posts

### Apply kebernetes configuration file
- kubectl apply -f posts-depl.yaml

### Apply all configuration files
- kubectl apply -f .

### Apply configuration modification and restart the deployment
- kubectl rollout restart deployment posts-depl

### Get services
- kubectl get services

### Get pods
- kubectl get pods

### Get logs
- kubectl logs comments-depl-5b9696f8f4-m4ksc

### ingress/nginx will help avoid manual docker build push and deployment

- https://kubernetes.github.io/ingress-nginx/deploy/
- kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.7.0/deploy/static/provider/cloud/deploy.yaml