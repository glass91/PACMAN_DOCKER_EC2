# PACMAN_DOCKER_EC2 #
# Docker Compose Setup for Pacman Game

# Pacman Game Setup with Docker Compose / Jenkins

Run the classic Pacman game using Docker Compose. This setup includes a Node.js-based Pacman application connected to a MongoDB database.

## Prerequisites

- **Docker**: Ensure Docker and Docker Compose are installed on your machine.
- **Initialization Script**: A `mongo-init-db` directory must exist in the same directory as your `docker-compose-deployment-pacman-and-mongo.yaml`. It should contain the `init_user_db.js` script for initializing the MongoDB database.

## Setup Instructions

### 1. Create a Network

Before deploying the services, create a dedicated network for them:

```bash
docker network create pacman-network
```
## start deployment 
docker compose -f docker-compose-deployment-pacman-and-mongo.yaml up -d
## stop deployment
3. docker compose -f docker-compose-deployment-pacman-and-mongo.yaml down
## Good Luck ##  :)))



PACMAN_DOCKER_EC2 Docker Compose Setup for Pacman Game Pacman Game Setup with Docker Compose / Jenkins Run the classic Pacman game using Docker Compose in AWS cloud. This setup includes a Node.js-based Pacman application connected to a MongoDB database.

Prerequisites Docker: Ensure Docker and Docker Compose are installed on your EC2 instancemachine. Initialization Script: A mongo-init-db directory must exist in the same directory as your docker-compose-deployment-pacman-and-mongo.yaml. It should contain the init_user_db.js script for initializing the MongoDB database. Setup Instructions

Create a Network Before deploying the services, create a dedicated network for them:
docker network create pacman-network start deployment docker compose -f docker-compose-deployment-pacman-and-mongo.yaml up -d

stop deployment docker compose -f docker-compose-deployment-pacman-and-mongo.yaml down

Containerization(Docker): doc-comp-pacman-DB.yaml IaaC (Terraform): data.tf, instances.tf, main.tf, outputs.tf, sg.tf CI/CD Pipeline(Jenkins): infra_setup_and_instance_setup copy.groovy, instance_tf_destroy.groovy Environment install automation (Ansible): playbook_pacman_docker.yaml
