🧩 Jenkins Job Chaining Project
🚀 Project Overview

This project demonstrates chaining multiple Jenkins jobs based on conditional triggers to simulate a complex DevOps pipeline.
It includes three main jobs:

Build Job – Compiles and prepares the project.

Test Job – Runs automated tests only if the build succeeds.

Deploy Job – Deploys the project automatically when tests pass.

The chaining is managed using Parameterized Trigger Plugin and conditional logic, simulating a real-world CI/CD pipeline.

🛠 Tools & Technologies

Jenkins (with plugins: Pipeline, Parameterized Trigger, Git)

Git & GitHub for source code management

Windows Batch Scripts for build and test steps

(Optional) Docker – for containerized deployment (can be added later)

⚙️ Workflow
Build Job  → (Success) →  Test Job  → (Success) →  Deploy Job


Each job triggers the next one only on success.

The pipeline simulates a real continuous integration flow.

🧱 How It Works

Build Job:

@echo off
echo Building...
ping -n 2 127.0.0.1
echo Build completed!
exit /b 0


Test Job:

@echo off
echo Testing...
ping -n 2 127.0.0.1 >nul
echo Tests completed successfully!
exit /b 0


Deploy Job:

@echo off
echo Deploying...
ping -n 2 127.0.0.1 >nul
echo Deployment completed!
exit /b 0

🧩 Features

✅ Conditional job chaining
✅ Automated execution using Git commits or manual builds
✅ Clear build-test-deploy flow
✅ Extendable for Docker or Kubernetes

📦 Future Enhancements

Add Docker container build and deployment.

Include Jenkinsfile (Declarative Pipeline format).

Integrate Slack/email notifications on job success or failure.

🧑‍💻 Author

Chowdavaram Jathin
💼 DevOps Enthusiast | 🧠 Learning CI/CD Automation
📬 Reach me at: chowdavramjathin@gmail.com
