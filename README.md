# 🚀 Automated Jenkins CI/CD Pipeline using GitHub & Python

## 📌 Project Description

This project demonstrates a complete Continuous Integration and Continuous Deployment (CI/CD) workflow using Jenkins integrated with GitHub.

The pipeline automatically triggers whenever code is pushed to the GitHub repository. Jenkins fetches the latest code, installs required dependencies, executes automated test cases using Pytest, and runs the Python application successfully.

This project helps in understanding DevOps automation, build pipelines, automated testing, and continuous delivery processes used in real-world software development environments.

---

# 🎯 Objectives

- Automate build and testing workflows
- Integrate Jenkins with GitHub
- Implement Continuous Integration (CI)
- Execute automated test cases
- Understand DevOps pipeline automation
- Reduce manual intervention in deployment workflows

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|----------|
| Jenkins | Automation Server |
| GitHub | Version Control Repository |
| Git | Source Code Management |
| Python | Application Development |
| Pytest | Automated Testing Framework |
| CI/CD | Build & Deployment Automation |

---

# 📂 Project Structure

```bash
automated-jenkin-project/
│
├── app.py
├── test_app.py
├── requirements.txt
├── Jenkinsfile
└── README.md
```

---

# ⚙️ Jenkins Pipeline Workflow

The Jenkins pipeline performs the following stages automatically:

## 1️⃣ Source Code Checkout
Jenkins fetches the latest source code from the GitHub repository.

## 2️⃣ Dependency Installation
Required Python libraries are installed using pip.

## 3️⃣ Automated Testing
Pytest framework executes automated test cases to validate the application.

## 4️⃣ Application Execution
After successful testing, the Python application is executed.

---

# 🔄 CI/CD Workflow Architecture

```text
Developer Pushes Code to GitHub
                ↓
        GitHub Repository
                ↓
      Jenkins Pipeline Triggered
                ↓
      Install Dependencies
                ↓
       Execute Test Cases
                ↓
        Run Application
                ↓
          Build Success
```

---

# 📜 Jenkinsfile

```groovy
pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\Aarya\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat '"C:\\Users\\Aarya\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" -m pytest'
            }
        }

        stage('Run Application') {
            steps {
                bat '"C:\\Users\\Aarya\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" app.py'
            }
        }
    }
}
```

---

# 📄 Application Code

## app.py

```python
print("Hello Jenkins CI/CD")
```

---

# 🧪 Automated Test Case

## test_app.py

```python
def test_sample():
    assert 10 == 10
```

---

# 📦 Requirements File

## requirements.txt

```text
pytest
```

---

# ▶️ How to Run Project Locally

## Step 1 — Clone Repository

```bash
git clone https://github.com/aarryya/automated-jenkin-project.git
```

---

## Step 2 — Navigate to Project Folder

```bash
cd automated-jenkin-project
```

---

## Step 3 — Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Step 4 — Run Test Cases

```bash
pytest
```

---

## Step 5 — Execute Application

```bash
python app.py
```

---

# 🚀 Features

✅ Automated CI/CD Pipeline  
✅ Jenkins Integration with GitHub  
✅ Automated Build Process  
✅ Automated Testing using Pytest  
✅ Continuous Integration Workflow  
✅ Pipeline as Code using Jenkinsfile  
✅ Faster Software Delivery Process  
✅ Reduced Manual Effort  

---

# 📸 Expected Jenkins Output

```text
Install Dependencies → SUCCESS
Run Tests → SUCCESS
Run Application → SUCCESS
Finished: SUCCESS
```

---

# 📚 Learning Outcomes

Through this project, the following concepts were learned:

- Jenkins Installation & Configuration
- GitHub Integration with Jenkins
- CI/CD Pipeline Development
- Automated Testing using Pytest
- Build Automation
- DevOps Workflow
- Pipeline as Code
- Webhook Trigger Concepts
- Continuous Integration Practices

---

# 🔮 Future Enhancements

- Docker Integration
- AWS EC2 Deployment
- Kubernetes Deployment
- Email Notifications
- Slack Integration
- Automated Deployment Pipeline
- Multi-Branch Pipeline Support

---

# 👨‍💻 Author

## Aarya Sawant

DevOps & Cybersecurity Enthusiast  
Passionate about CI/CD Automation, Cloud Computing, and Infrastructure Automation.

---

# ⭐ Conclusion

This project successfully demonstrates the implementation of an automated Jenkins CI/CD pipeline integrated with GitHub. It automates code integration, testing, and execution workflows, helping developers achieve faster and more reliable software delivery with minimal manual intervention.
