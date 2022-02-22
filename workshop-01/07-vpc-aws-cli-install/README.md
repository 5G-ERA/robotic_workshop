# VPC aws-cli install
| [Previous](../06-vpc-docker-install/README.md) | [index](../README.md) | [next](../08-registry-creation/README.md) |
| :--- | :--: | ---: |

[commands](07-vpc-aws-cmd.txt)

## Install aws-cli

```bash
sudo apt install -y unzip
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
aws --version
rm awscliv2.zip
```


<img src="07-vpc-aws-00.png"/>
<img src="07-vpc-aws-01.png"/>

## Getting credentials 


<img src="07-vpc-aws-02.png"/>
<img src="07-vpc-aws-03.png"/>
<img src="07-vpc-aws-04.png"/>
<img src="07-vpc-aws-05.png"/>

## Configuring aws-cli credentials

```bash
aws configure
```

<img src="07-vpc-aws-06.png"/>

| [Previous](../06-vpc-docker-install/README.md) | [index](../README.md) | [next](../08-registry-creation/README.md) |
| :--- | :--: | ---: |
