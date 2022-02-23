# VPC docker engine install
| [Previous](../06-deploy-robot-simulation/README.md) | [index](../README.md) | [next](../08-vpc-aws-cli-install/README.md) |
| :--- | :--: | ---: |

[commands](07-vpc-docker-cmd.txt)

## VPC access

<img src="07-vpc-docker-00.png"/>
<img src="07-vpc-docker-01.png"/>
<img src="07-vpc-docker-02.png"/>
<img src="07-vpc-docker-03.png"/>

## Docker install

```bash
sudo snap install docker
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker
sudo reboot
```
<img src="07-vpc-docker-04.png"/>

## Docker installation check

```bash
docker run hello-world
```
<img src="07-vpc-docker-05.png"/>

| [Previous](../06-deploy-robot-simulation/README.md) | [index](../README.md) | [next](../08-vpc-aws-cli-install/README.md) |
| :--- | :--: | ---: |
