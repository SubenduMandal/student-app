# 🚀 Student Management Web App (DevOps Project)

## 📌 Project Overview

This project demonstrates a **Cloud-based DevOps pipeline** by building and deploying a **Student Management Web Application** using modern DevOps tools.

The application allows users to:

* ➕ Add students
* 📋 View student records
* ❌ Delete students

The main objective is to showcase **CI/CD automation, containerization, orchestration, and monitoring** in a real-world workflow.

---

## 🧩 DevOps Pipeline (4 Stages)

```
1. Source  → GitHub
2. Build   → Jenkins + Docker
3. Deploy  → Kubernetes (AWS / Minikube)
4. Monitor → Nagios
```

---

## 🔄 Workflow Architecture

```
Developer → GitHub → Jenkins → Docker → Kubernetes → AWS
                                      ↓
                                   Nagios
```

---

## 🛠️ Technologies Used

* Backend: Python (Flask)
* Frontend: HTML, CSS
* Database: SQLite
* Version Control: Git & GitHub
* CI/CD Tool: Jenkins
* Containerization: Docker
* Orchestration: Kubernetes
* Cloud Platform: AWS
* Monitoring Tool: Nagios

---

## 📁 Project Structure

```
student-app/
│
├── app/
│   ├── app.py
│   ├── requirements.txt
│   └── templates/
│       └── index.html
│
├── docker/
│   └── Dockerfile
│
├── jenkins/
│   └── Jenkinsfile
│
├── k8s/
│   ├── deployment.yaml
│   └── service.yaml
│
├── monitoring/
│   └── nagios.conf
│
├── README.md
└── .gitignore
```

---

## ⚙️ Setup & Installation (Local)

### 1. Clone Repository

```bash
git clone https://github.com/your-username/student-app.git
cd student-app/app
```

### 2. Run Application

```bash
python3 app.py
```

Open in browser:

```
http://localhost:5000
```

---

## 🐳 Docker Setup

### Build Image

```bash
docker build -t student-app ./docker
```

### Run Container

```bash
docker run -p 5000:5000 student-app
```

---

## ⚙️ Jenkins CI/CD Pipeline

* Pulls code from GitHub
* Builds Docker image
* Runs container automatically

Pipeline defined in:

```
jenkins/Jenkinsfile
```

---

## ☸️ Kubernetes Deployment

### Apply Configurations

```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
```

### Access Application

```bash
minikube service student-service
```

---

## ☁️ AWS Deployment (Concept)

* Deploy using EC2 or EKS
* Kubernetes manages scaling and availability

---

## 📊 Monitoring with Nagios

Nagios is used to monitor:

* Server uptime
* CPU & memory usage
* Application availability

---

## 🎯 Key DevOps Concepts Demonstrated

* Continuous Integration (CI)
* Continuous Deployment (CD)
* Containerization using Docker
* Orchestration using Kubernetes
* Infrastructure on Cloud (AWS)
* Monitoring & Alerting

---

## 🚀 Future Enhancements

* Add authentication (login system)
* Use MySQL/PostgreSQL instead of SQLite
* Integrate Docker Hub for image storage
* Add Prometheus & Grafana for advanced monitoring
* Implement auto-scaling in Kubernetes

---

## 👨‍💻 Author

**Subendu Mandal**
M.Tech (Computer Science Engineering - Software Engineering)

---

## 📢 Conclusion

This project successfully demonstrates a **complete DevOps lifecycle**, from development to deployment and monitoring, using industry-standard tools.

---
