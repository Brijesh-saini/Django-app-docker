# Django Notes App with Docker

This repository contains a containerized Django application using Docker and Docker Compose. The architecture includes an Nginx reverse proxy, a Django backend served by Gunicorn, and a MySQL database.

## Architecture

* **Nginx** (`nginx_cont`): Acts as a reverse proxy, listening on port 80 and routing traffic to the Django backend.
* **Django** (`django_cont`): The core application, served via Gunicorn on port 8000. It automatically runs database migrations on startup.
* **MySQL** (`db_cont`): The database server, running on port 3306. Data is persisted locally using a volume.

## Prerequisites

Before you begin, ensure you have the following installed on your machine:
* [Docker](https://docs.docker.com/get-docker/)
* [Docker Compose](https://docs.docker.com/compose/install/)
* Git

## 🚀 Setup & Installation

### 1. Clone the Repository
Clone this repository to your local machine:
```bash
git clone [https://github.com/Brijesh-saini/Django-app-docker.git](https://github.com/Brijesh-saini/Django-app-docker.git)
cd Django-app-docker
