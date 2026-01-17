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


    1  ls -ltr
    2  sudo kubectl version
    3  sudo kubectl get ns
    4  sudo vim pod.yml
    5  sudo vim ns.yml
    6  ls
    7  sudo kubectl apply -f pod.yml
    8  sudo kubectl get ns
    9  sudo kubectl apply -f ns.yml
   10  sudo kubectl get ns
   11  sudo kubectl get pod
   12  histroy
   13  history
   14  sudo kube get pod
   15  sudo kubectl get pod
   16  sudo kubectl get ns
   17  ls -ltr
   18  sudo cat ns.yml
   19
   20  sudo cat pod.yml
   21  ls
   22  sudo vim replicaset.yml
   23  sudo kubectl get ns
   24  sudo kubectl get pod
   25  sudo kubectl delete pod/nginx-pod
   26  sudo kubectl get pod
   27  sudo kubectl apply -f replicaset.yml -n prod-ns
   28  ls -ltr
   29  sudo cat ns.yml
   30  sudo kubectl get ns
   31  sudo kubectl get -n prod-ns
   32  sudo kubectl pod -n prod-ns
   33  sudo kubectl get pod -n prod-ns
   34  sudo kubectl get all -n prod-ns
   35  history
   36  ls -ltr
   37
   38  sudo kubectl get all -n prod-ns
   39  sudo kubectl delete replicaset.apps/nginx-replicaset -n prod-ns
   40  sudo kubectl get all -n prod-ns
   41  sudo vim deployment.yml
   42  sudo kubectl apply -f deployment.yml -n dev-ns
   43  sudo kubectl get all -n dev-ns
   44  ls
   45  cat ns.yml
   46  cat pod.yml
   47  cat replicaset.yml
   48  cat deployment.yml
   49  history
