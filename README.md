# open-cluster-management(Ubuntu)
## Install kubectl
```
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
kubectl version --client
```
## Install Golang,kind,docker,ocm
```
snap install go --classic
go install sigs.k8s.io/kind@v0.20.0
vi ~/.bashrc # add PATH=$PATH:/root/go/bin and run source ~/.bashrc command
snap install docker
curl -L https://raw.githubusercontent.com/open-cluster-management-io/OCM/main/solutions/setup-dev-environment/local-up.sh | bash
```
