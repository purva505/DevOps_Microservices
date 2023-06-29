

GIT HUB PROJECT LINK :https://github.com/purva505/DevOps_Microservices.git

1--> https://github.com/purva505/DevOps_Microservices.git
	Branch : main
All changes are done in main branch

2--> app.py file updated to print required logs

3--> Installed kubectl utility and minikube using necessary command

kubectl installation:

curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
kubectl version --client

minikube installation:

curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube

4--> Run minikube start command

5--> Edited Dockerfile, run_docker.sh and checked it using make lint command 

hadolint Dockerfile
make lint
./run_docker.sh
open new terminal and run command ./make_prediction.sh
./make_prediction.sh > docker_out.txt

6--> Run upload_docker.sh command to upload the newly created image to the docker hub

7--> Edited run_kuberntes.sh and run below command

./run_kuberntes.sh 
open new terminal and run command ./make_prediction.sh
./make_prediction.sh > kubernetes_out.txt


