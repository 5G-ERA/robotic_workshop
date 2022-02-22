# ROS node example kubernetes deployment
| [Previous](../09-docker-image-creation/README.md) | [index](../README.md) | [next](../11-deploy-robot-simulation/README.md) |
| :--- | :--: | ---: |

[commands](10-deploy-image-cmd.txt)

## Applying the manifest files

```bash

git clone https://github.com/5G-ERA/ros_docker_image_example.git
cd "ros_docker_image_example"
cd k8s
kubectl apply -f talker.yaml
kubectl apply -f listener.yaml
```

<img src="10-deploy-image-00.png"/>

## Checking that everything is running

```bash
kubectl get pods
```

<img src="10-deploy-image-01.png"/>

## Checking the interaction

```bash
kubectl logs -l app=talker-pod
kubectl logs -l app=listener-pod
```

<img src="10-deploy-image-02.png"/>

| [Previous](../09-docker-image-creation/README.md) | [index](../README.md) | [next](../11-deploy-robot-simulation/README.md) |
| :--- | :--: | ---: |
