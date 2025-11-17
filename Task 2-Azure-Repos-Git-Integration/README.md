# 🟦 Task 2 — Create & Manage Azure Repos (Git Integration)

## 📌 Objective
To configure and link **Azure DevOps Repos** with **local Git (Git Bash)** for seamless version control.  
This task demonstrates secure authentication using a **Personal Access Token (PAT)**, cloning the repository locally, committing changes, and pushing updates back to Azure DevOps — completing a full DevOps workflow from **local system → cloud repo**.

---

## ⚙️ Tools & Services Used
- **Azure DevOps Repos** — Cloud Git repository  
- **Git Bash** — Local Git command-line tool  
- **Personal Access Token (PAT)** — Secure authentication  
- **Windows 10** — Local development environment  

---

## 🪜 Steps Executed

### 🔹 Step 1 — Create Azure DevOps Repository
- Logged into **https://dev.azure.com**
- Opened the existing project: **AravindAzureLab**
- Navigated to **Repos → Files**
- Initialized repository using **Add README.md**
- Verified default branch: `main`

---

### 🔹 Step 2 — Copy Repository Clone URL
- Clicked **Clone** in Azure DevOps  
- Selected **HTTPS**  
- Copied the clone URL: https://dev.azure.com/geedulaaravind/AravindAzureLab/_git/AravindAzureLab

- 
---

### 🔹 Step 3 — Configure Git Locally
- Installed **Git for Windows**
- Verified installation:

```bash
git --version

Created a working directory:
mkdir AzureDevOpsProjects
cd AzureDevOpsProjects

Step 4 — Clone Azure DevOps Repository
git clone https://dev.azure.com/geedulaaravind/AravindAzureLab/_git/AravindAzureLab
During first authentication, created a Personal Access Token (PAT)

Scope: Code (Read & Write)

Entered PAT as password

Clone successful:
Cloning into 'AravindAzureLab'...
Receiving objects: 100%
Resolving deltas: 100%

Step 5 — Create & Commit a New File

Entered project directory:
cd AravindAzureLab
Created a new file:
"This is Task 2 test file" > task2.txt
Staged & committed:

git add .
git commit -m "Added task2.txt for DevOps Task 2"

Step 6 — Push to Azure DevOps

Pushed changes:
git push
To https://dev.azure.com/geedulaaravind/AravindAzureLab/_git/AravindAzureLab
main -> main


Outcome

Successfully connected local Git with Azure DevOps Repos

Secured authentication using PAT

Verified commit → push → sync workflow

Completed a real-world DevOps version control cycle





