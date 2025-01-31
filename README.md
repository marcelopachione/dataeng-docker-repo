# Data Engineering Docker Repository

This repository contains configurations for creating and managing a modern data stack environment using **Docker**.

## 🌐 Available Environments

| Environment   | Description                                     | Start Command                                      | Stop Command |
|--------------|-----------------------------------------------|---------------------------------------------------|--------------|
| PostgreSQL + PgAdmin | Relational database and administration tool | `docker-compose -f postgres/docker-compose.yml up -d` | `docker-compose -f postgres/docker-compose.yml down` |
| Spark Cluster | Apache Spark cluster with 2 worker nodes | `docker-compose -f spark/docker-compose.yml up -d --scale spark-worker=2` | `docker-compose -f spark/docker-compose.yml down` |

---

## 📌 Requirements  
- **Docker** and **Docker Compose** installed  
- Configuration files for **PostgreSQL** and **Spark** in the respective directories  

## 📎 Additional Information  
- To check container logs:  
  ```sh
  docker logs <container_name>
  ```
- To access a running container:  
  ```sh
  docker exec -it <container_name> /bin/bash
  ```
