# kubectl install on AWS Cloud Console
| [Previous](../03-creating-worker-nodes/README.md) | [index](../README.md) | [next](../05-metrics-server/README.md) |
| :--- | :--: | ---: |

[commands](04-kubectl-cmd.txt)

## Create the AWS console 

<img src="04-kubectl-00.png"/>
<img src="04-kubectl-01.png"/>
<img src="04-kubectl-02.png"/>

## Install kubectl

```bash
curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.21.2/2021-07-05/bin/linux/amd64/kubectl
chmod +x ./kubectl
mkdir bin
mv kubectl bin
kubectl version
```

<img src="04-kubectl-03.png"/>

## Configure cluster access
```bash
aws eks update-kubeconfig --region eu-central-1 --name 5g-era-robotic-workshop-cluster
kubectl get nodes
```
<img src="04-kubectl-04.png"/>

| [Previous](../03-creating-worker-nodes/README.md) | [index](../README.md) | [next](../05-metrics-server/README.md) |
| :--- | :--: | ---: |
