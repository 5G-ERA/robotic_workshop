# VPC docker engine install
| [Previous](../05-metrics-server/README.md) | [index](../README.md) | [next](../07-vpc-aws-cli-install/README.md) |
| :--- | :--: | ---: |

[commands](06-vpc-docker-cmd.txt)

## VPC access

<img src="06-vpc-docker-00.png"/>
<img src="06-vpc-docker-01.png"/>
<img src="06-vpc-docker-02.png"/>
<img src="06-vpc-docker-03.png"/>

## Docker install

```bash
sudo snap install docker
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker
sudo reboot
```
<img src="06-vpc-docker-04.png"/>

## Docker installation check

```bash
docker run hello-world
```
<img src="06-vpc-docker-05.png"/>

| [Previous](../05-metrics-server/README.md) | [index](../README.md) | [next](../07-vpc-aws-cli-install/README.md) |
| :--- | :--: | ---: |
