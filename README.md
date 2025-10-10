# Vite App – CI/CD Pipeline Project

## 📌 Project Description
This is a simple **Vite application** containerized with Docker and deployed using a **CI/CD pipeline**.  
The pipeline is automated using **GitHub Actions**, which builds the Docker image, pushes it to **Docker Hub**, and can deploy it on an **AWS EC2 instance**.

---

## ⚙️ CI/CD Pipeline Workflow
The GitHub Actions workflow (`.github/workflows/ci-cd.yml`) performs the following steps:

1. **Build** → Builds a Docker image from the Vite app.  
2. **Test** → (Optional) Runs simple checks or tests.  
3. **Push** → Pushes the Docker image to **Docker Hub**.  
4. **Deploy** → Deploys the app to **AWS EC2** using Docker.  

### 🔄 Triggers
The pipeline runs automatically when:
- Code is **pushed to the `main` branch**  
- OR a **pull request is merged** into `main`  

---

## 🚀 How to Run Locally
1. Clone this repository:
   ```bash
   git clone https://github.com/HajiraImran/DevOpsPeoject.git
   cd my-app
