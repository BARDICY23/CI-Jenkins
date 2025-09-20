# CI/CD Pipeline with Jenkins, SonarQube, Nexus, and Slack

This project showcases a **CI/CD pipeline** implementation where I handled the **infrastructure setup** and **DevOps tooling integration**.  
The Java application included in the repo is for demonstration purposes only — my responsibility was building the pipeline and configuring the supporting services.

---

## 🚀 Pipeline Overview

The Jenkins pipeline is defined in the `Jenkinsfile` and integrates multiple stages to ensure smooth CI/CD:

1. **Build**
   - Compiles the project and packages the application (WAR).

2. **Test**
   - Runs unit tests with reports generated.

3. **Checkstyle**
   - Performs static code style checks.

4. **SonarQube Analysis**
   - Scans code for bugs, vulnerabilities, and coverage.
   - Uses JaCoCo for test coverage reports.

5. **Quality Gate**
   - Enforces SonarQube quality gates (pipeline stops if it fails).

6. **Artifact Upload**
   - Uploads the build artifact (WAR) to **Nexus Repository Manager**.

7. **Slack Notification**
   - Sends build status (success/failure) to a Slack channel.

---

## 🛠️ Tools & Services Used

- **Jenkins** → Orchestrates the pipeline.  
- **SonarQube** → Code analysis and quality gates.  
- **Nexus Repository Manager** → Stores build artifacts.  
- **Slack** → Build notifications.  
- **Maven** → Build tool for dependency management and packaging.  
- **GCP VMs** → Hosting Jenkins, Nexus, and SonarQube servers.

---

## 📂 Repo Structure

- `Jenkinsfile` → Defines CI/CD pipeline stages.  
- `settings.xml` → Maven settings for Nexus repository integration.  
- `gcloud-cli-setup/README.md` → Separate documentation for infrastructure automation (VMs, firewall rules).  

---

## ✅ What I Worked On

- Provisioned cloud infrastructure for Jenkins, SonarQube, and Nexus.  
- Configured **firewall rules, VM startup scripts, and private/public access rules**.  
- Installed and configured **Jenkins, SonarQube, Nexus, and Slack integration**.  
- Built and tested a **production-style CI/CD pipeline**.  

---

## 📲 Notifications

Slack integration provides instant feedback:
- ✅ Success → Green notification  
- ❌ Failure → Red notification  

---

## ⚠️ Note

I am **not responsible for the Java/Spring application code** itself — my work was focused on the **infrastructure, CI/CD pipeline, and DevOps tooling setup**.

