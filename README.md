# Softy Pinko Docker Project

## 🌐 Description
This project demonstrates the step-by-step containerization of a full-stack web application using **Docker** and **Docker Compose**. It showcases the evolution from manual container management to a professional, scalable 3-tier architecture featuring a reverse proxy and load balancer.

---

## 🏗️ Infrastructure Architecture
The final stage of this project (Task 6) implements a robust infrastructure where all traffic is unified through a single entry point:

* **Proxy Server (Nginx):** Acts as a Reverse Proxy and Load Balancer (listening on Port 80).
* **Front-end Server (Nginx):** A static web server hosting the HTML/CSS/JS files.
* **Back-end Server (Flask):** A Python API that provides dynamic data.



---

## 📅 Task Breakdown

| Task | Title | Key Learning Objectives |
| :--- | :--- | :--- |
| **0** | **Docker Image** | Creating a basic Ubuntu-based image and understanding `Dockerfile` syntax. |
| **1** | **Back-end** | Containerizing a Flask API, installing Python dependencies, and port mapping. |
| **2** | **Front-end** | Using Nginx to serve static content and setting up custom `.conf` files. |
| **3** | **Integration** | Connecting tiers using AJAX and resolving CORS (Cross-Origin Resource Sharing) issues. |
| **4** | **Orchestration** | Using `docker-compose.yml` to manage multiple containers with one command. |
| **5** | **Proxy Server** | Implementing a Reverse Proxy to hide internal ports and unify the URL structure. |
| **6** | **Scale Horizontally** | Scaling the API tier and observing Round-Robin Load Balancing in action. |

---

## 🚀 Getting Started

### Prerequisites
* **Docker Desktop** (Ensure the Docker Daemon is running).
* **Git** installed on your local machine.

### Installation & Setup
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/agalotaibi/holbertonschool-softy-pinko-docker.git](https://github.com/agalotaibi/holbertonschool-softy-pinko-docker.git)
   cd holbertonschool-softy-pinko-docker

2. **Navigate to the latest task:**
   ```bash
   cd task6
   
3. **Running the Project:**
     ```bash
     To build and start the entire infrastructure:
           docker-compose up --build

     To scale the back-end to multiple instances:
          docker-compose up --scale back-end=2


## 🔗 Usage
Once the containers are active, you can access the project through the Proxy:

Main Website: http://localhost

API Hello Route: http://localhost/api/hello

Note: Accessing port 5252 or 9000 directly will fail by design, as these are now protected behind the proxy "firewall."

## 🛠️ Tech Stack
OS: Ubuntu

Web Servers: Nginx

Language: Python 3

Framework: Flask

Orchestration: Docker Compose

## 👤 Author

Amaal AlOtaibi
