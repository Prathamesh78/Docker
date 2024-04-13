
# Docker Commands

This repository contains descriptions and examples of various Docker commands commonly used in container management and orchestration.

## Prerequisites

Before running any Docker commands, ensure that Docker is installed on your system. You can check the version of Docker installed using the following command:

```bash
docker --version
```

## Managing Docker Service

### Checking Docker Service Status

To check the status of the Docker service, use:

```bash
systemctl status docker
```

### Starting Docker Service

To start the Docker service, use:

```bash
systemctl start docker
```

### Stopping Docker Service

To stop the Docker service, use:

```bash
systemctl stop docker
```

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

### Pulling and Running an Nginx Container with Tag

To pull an Nginx image with a specific tag and run a container, use:

```bash
docker pull nginx:latest
docker run nginx:latest
```

## Contributing

Contributions are welcome! If you have any improvements or additional Docker commands to add, feel free to submit a pull request.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
