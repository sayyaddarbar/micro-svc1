CI:
Dockerbuild:
    aws ecr login | docker login
    docker build -t ecrRepourl:tag
    dockerr push ecrRepourl:tag
CD: 
kubectl apply -f deployment.yaml service.yaml ingress.yaml

jenkins