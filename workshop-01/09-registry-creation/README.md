# Elastic Container Registry (ECR) creation
| [Previous](../08-vpc-aws-cli-install/README.md) | [index](../README.md) | [next](../10-docker-image-creation/README.md) |
| :--- | :--: | ---: |

[commands](09-registry-cmd.txt)

## Creating the registry
<img src="09-registry-00.png"/>
<img src="09-registry-01.png"/>
<img src="09-registry-02.png"/>
<img src="09-registry-03.png"/>
<img src="09-registry-04.png"/>
<img src="09-registry-05.png"/>
<img src="09-registry-06.png"/>
<img src="09-registry-07.png"/>
<img src="09-registry-08.png"/>
<img src="09-registry-09.png"/>

## Giving access to the registry to VPC

```bash
aws ecr get-login-password --region eu-central-1 | \
docker login --username AWS --password-stdin 394603622351.dkr.ecr.eu-central-1.amazonaws.com
```

<img src="09-registry-10.png"/>

| [Previous](../08-vpc-aws-cli-install/README.md) | [index](../README.md) | [next](../10-docker-image-creation/README.md) |
| :--- | :--: | ---: |
