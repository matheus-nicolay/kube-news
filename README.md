# Projeto Kube-news
Aplicação desenvolvida em NodeJS para *deploy*, com o objetivo de construir um projeto completo de automação DevOps.

### Funcionalidades:
- **src/Dockerfile**
  - Definição da imagem Docker para a aplicação

- **deploy-prometheus-grafana.yaml**
    Arquivo de deployment Kubernetes
    
  - Deploy do Prometheus 
  - Deploy do Grafana

- **k8s/deployments.yaml**
    Arquivo de deployment Kubernetes
    
  - Deployment da aplicação (com imagem personalizado do Docker Hub) 
  - Deployment do banco de dados PostgreSQL
  - Service loadbacing

- **Jenkinsfile**
   Pipeline Jenkins para deploy automatizado da aplicação dentro do cluster Kubernetes
   
  - Gerar imagem docker da aplicação
  - Efetuar o *push* da imagem no Docker Hub   
  - Ativar o *deployment* do Kubernetes
