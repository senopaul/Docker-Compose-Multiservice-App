# Multi-Service Web Application Stack with Docker Compose

## Overview

This project provides a production-ready, multi-service web application stack orchestrated using Docker Compose. It integrates essential components for modern web applications, including:

- **MySQL**: Relational database for persistent data storage  
- **Memcached**: In-memory caching for fast data retrieval  
- **RabbitMQ**: Message broker for reliable inter-service communication  
- **Tomcat**: Java application server for deploying web applications  
- **Nginx**: Web server and reverse proxy for serving static content and load balancing

This stack is ideal for learning, prototyping, or as a foundation for enterprise-grade web applications.

---

## Features

- **Modular Architecture**: Each service runs in its own container for easy management and scaling.
- **Data Persistence**: Volumes ensure important data is retained across container restarts.
- **Network Isolation**: All services communicate over a dedicated Docker network.
- **Ready for Development & Production**: Easily extend or customize for your needs.

---

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/products/docker-desktop)
- [Docker Compose](https://docs.docker.com/compose/)

### Quick Start

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/docker-webapp-stack.git
   cd docker-webapp-stack
   ```

2. **Start all services:**
   ```sh
   docker-compose up -d
   ```

3. **Access the services:**
   - **MySQL**: Connect with a client at `localhost:3306` (user: `myuser`, password: `mypassword`)
   - **RabbitMQ Management UI**: [http://localhost:15672](http://localhost:15672) (user: `myuser`, password: `mypassword`)
   - **Tomcat**: [http://localhost:8080](http://localhost:8080)
   - **Nginx**: [http://localhost:8081](http://localhost:8081)

---

## Project Structure

```
.
├── app/                # Java web application files for Tomcat
├── db_data/            # MySQL data (persisted)
├── web/                # Static web content for Nginx
├── docker-compose.yml  # Main Docker Compose configuration
└── ...
```

---

## Customization

- **Add your Java webapps** to `app/webapps/` for Tomcat deployment.
- **Place static HTML files** in `web/html/` for Nginx.
- **Modify environment variables** in `docker-compose.yml` as needed.

---

## License

This project is licensed under the MIT License.

---

## Contact

For questions or collaboration, please contact [your-email@example.com](mailto:your-email@example.com).

---

> **Empower your development with a robust, scalable, and modular Docker-based web application stack.**


