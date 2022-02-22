# ROS node example image build
| [Previous](../09-deploy-robot-simulation/README.md) | [index](../README.md) | [next](../11-image-deployment/README.md) |
| :--- | :--: | ---: |

[commands](10-docker-image-cmd.txt)

## Getting the dockerfiles

```bash
git clone https://github.com/5G-ERA/ros_docker_image_example.git
cd "ros_docker_image_example"
aws_reg="394603622351.dkr.ecr.eu-central-1.amazonaws.com"
registry="robotic-workshop-01"
image="${registry}"
version="ros-example-test"
image_name="${image}:${version}"
full_tag="${aws_reg}/${image_name}"
```


<img src="10-docker-image-00.png"/>

## Building the image

```bash
docker build -t "${image_name}" .
```


## Pushing the image to the registry

```bash
docker tag "${image_name}" "${full_tag}"
docker push "${full_tag}"
```

<img src="10-docker-image-01.png"/>

| [Previous](../09-deploy-robot-simulation/README.md) | [index](../README.md) | [next](../11-image-deployment/README.md) |
| :--- | :--: | ---: |
