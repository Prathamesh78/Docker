![image](https://github.com/Prathamesh78/Docker/assets/104883046/0d7fded4-8ce8-464b-8fa9-18c9e11bcbc0)
# Docker Commands

This repository contains descriptions and examples of various Docker commands commonly used in container management and orchestration.

## Prerequisites

Before running any Docker commands, ensure that Docker is installed on your system. You can check the version of Docker installed using the following command:

```bash
docker --version
```
![image](https://github.com/Prathamesh78/Docker/assets/104883046/b24eb6c7-2e57-47ae-b47c-dc84b369be8c)

## Managing Docker Service

### Checking Docker Service Status

To check the status of the Docker service, use:

```bash
systemctl status docker
```
![image](https://github.com/Prathamesh78/Docker/assets/104883046/ab1a449b-aa86-49fc-b59b-03e79f4128df)

### Starting Docker Service

To start the Docker service, use:

```bash
systemctl start docker
```
![image](https://github.com/Prathamesh78/Docker/assets/104883046/11e86626-8a86-42de-8759-a772347a56ef)

### Stopping Docker Service

To stop the Docker service, use:

```bash
systemctl stop docker
```
![image](https://github.com/Prathamesh78/Docker/assets/104883046/ab34fde0-1cc8-4898-95f8-4d3f1921aae1)

![image](https://github.com/Prathamesh78/Docker/assets/104883046/a8410e21-4720-42d4-a002-7b498fb4f562)

### Restarting Docker Service

To restart the Docker service, use:

```bash
systemctl restart docker
```

### Enabling Docker Service

To enable the Docker service to start on boot, use:

```bash
systemctl enable docker
```

## Working with Docker Images

### Listing Images

To list the images present on the local machine, use:

```bash
docker images
```
![image](https://github.com/Prathamesh78/Docker/assets/104883046/f0e4272a-67f3-4f0f-9fb2-57b0fad49323)

## Managing Docker Containers

### Listing Running Containers

To list containers that are in the running state, use:

```bash
docker ps
```

### Listing All Containers

To list all containers, including those in the running and stopped/exited states, use:

```bash
docker ps -a
```
![image](https://github.com/Prathamesh78/Docker/assets/104883046/7a2a8a78-0189-4654-a9b3-33a32a117f97)

### Pulling Images from Docker Hub

To download container images from Docker Hub registry to the local machine, use:

```bash
docker pull <image_name>
```

### Running Containers

To create and run a container based on an image, use:

```bash
docker run <image_name>
```

### Running Containers with Tag

To specify a tag while pulling an image or running a container, use:

```bash
docker pull <image_name>:<tag>
docker run <image_name>:<tag>
```

Replace `<image_name>` with the name of the Docker image and `<tag>` with the specific version or tag of the image.

## Examples

### Pulling and Running an Ubuntu Container

To pull the Ubuntu image from Docker Hub and run a container, use:

```bash
docker pull ubuntu
docker run ubuntu
```
![image](https://github.com/Prathamesh78/Docker/assets/104883046/68bf60d3-7f93-4c13-9d2d-9faff3d7bead)

![image](https://github.com/Prathamesh78/Docker/assets/104883046/073c1bd0-3933-433f-a0d3-2321f0a76475)

### Pulling and Running an Nginx Container with Tag

To pull an Nginx image with a specific tag and run a container, use:

```bash
docker pull nginx:1.25.4
docker run nginx:1.25.4
```
![image](https://github.com/Prathamesh78/Docker/assets/104883046/bc91ff15-b190-4426-9c81-007027072b04)

![image](https://github.com/Prathamesh78/Docker/assets/104883046/a4542080-4561-4e12-a4f0-e1862b330cab)

## Contributing

Contributions are welcome! If you have any improvements or additional Docker commands to add, feel free to submit a pull request.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
