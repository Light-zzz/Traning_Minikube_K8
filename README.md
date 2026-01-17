# Traning_Minikube_K8
This is only for practice for Kubernetes


**Installation of Docker and Minikube**

Updating Linux: sudo yum update -y

Install Docker: sudo yum install docker* -y

Start docker: sudo systemctl start docker
Status docker: sudo systemctl status docker

Download Minikube Repo: sudo curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64

Install Minikube: sudo install minikube-linux-amd64 /usr/local/bin/minikube

Check Minikube version: minikube version

Start the minikube: sudo minikube start --driver=docker --force

Download Kubernetes repo: sudo curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl

Give the permission to kubernetes: chmod +x ./kubectl

Move kubernets: sudo mv ./kubectl /usr/local/bin/kubectl

Check Kubernetes version: kubectl version

Verify the Kubernets verion yaml: kubectl version --output=yaml

Check the kubernets nodes: sudo kubectl get nodes

Kubectl Commands in minikube:

1. sudo kubectl get ns
2. sudo kubectl
3. 
