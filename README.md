# Demo Python CI/CD Pipeline using Jenkins

## Project Overview
This project is a **basic demonstration of a CI/CD pipeline** using **Jenkins** for running **Python tests**.

The main goal of this project was to:
- Install and configure **Jenkins**
- Create a **Jenkins pipeline**
- Integrate **Python testing using pytest**
- Understand CI/CD concepts through multiple pipeline failures and fixes
- Successfully achieve a **working pipeline execution**

This project focuses on **learning Jenkins and CI/CD fundamentals**, not on application complexity.

---

## Technologies Used
- Jenkins (running inside Docker)
- Docker
- Python 3
- Pytest
- Git & GitHub
- Linux (Arch Linux host)

---

## Project Structure
.
├── Jenkinsfile
├── README.md
├── ops.py
├── test_ops.py


---

## Jenkins Setup
- Jenkins is run **inside a Docker container**
- Jenkins UI is accessed via:
- Pipeline configuration is defined using a `Jenkinsfile` stored in the repository

---

## CI/CD Pipeline Flow
The Jenkins pipeline performs the following steps:

1. **Checkout Source Code**
 - Clones the repository from GitHub

2. **Environment Setup**
 - Prepares Python environment
 - Installs required testing dependencies

3. **Test Execution**
 - Executes Python test cases using `pytest`

4. **Pipeline Result**
 - Pipeline fails if tests fail
 - Pipeline succeeds when all tests pass

---

## Challenges Faced
During the setup, several issues were encountered:
- Jenkins startup and configuration problems
- Python dependency installation errors
- `pip` restrictions due to newer Python packaging rules (PEP 668)
- Multiple pipeline failures at different stages
- Environment-related issues inside Docker

These failures helped in understanding:
- Jenkins pipeline stages
- CI/CD troubleshooting
- Dependency management
- Jenkins logs and console output

---

## Final Outcome
After resolving the issues step by step:
- Jenkins pipeline executed successfully
- Python tests ran correctly using pytest
- The CI/CD pipeline completed with a **successful build**

A screenshot of the successful pipeline execution is included below.

---

## Screenshot

<img width="1913" height="528" alt="Screenshot From 2026-01-16 02-27-56" src="https://github.com/user-attachments/assets/48124704-d795-4179-a0f0-2b2bc16fb1ac" />

<img width="1901" height="942" alt="image" src="https://github.com/user-attachments/assets/2735b586-b08f-4f61-bc68-52581948ba2a" />




---

## Conclusion
This project provided hands-on experience with:
- Jenkins CI/CD pipelines
- Docker-based Jenkins setup
- Python test automation
- Debugging real CI/CD pipeline failures

It serves as a **simple and effective demonstration** of a Python CI/CD pipeline using Jenkins.
