# Dockerized Apache-PHP-MySQL Setup

This project sets up a Docker environment for running Apache, PHP, and MySQL services. It allows you to quickly spin up a development environment for web applications.

## Components

- **Apache:** Web server handling HTTP requests.
- **PHP:** Server-side scripting language for web development.
- **MySQL:** Relational database management system.

## Setup

1. **Clone the Repository:** Clone this repository to your local machine.

    ```bash
	git clone https://github.com/Sprysio/docker-lamp.git
    ```

2. **Build and Run Docker Containers:**

    ```bash
    docker-compose up --build
    ```

3. **Accessing Services:**

    - **Apache:** Access your web server at `http://localhost:6666`
    - **PHP:** No direct access. Used by Apache.
    - **MySQL:** Access MySQL at `localhost:8889`

## Project Structure

- `docker-compose.yml`: Defines services, networks, and volumes for Docker containers.
- `apache/`, `php/`, `mysql/`: Directories containing Dockerfiles for each service.
- `www/`: Directory for web application files.
- `apache/apache-vhost.conf`: Apache virtual host configuration.
- `www/index.php`: Sample PHP file for testing.
