Task 2 — Create & Manage Azure Repos (Git Integration)
📌 Objective

Configure and link Azure DevOps Repos with local Git (Git Bash) for seamless version control.
This includes authentication using a Personal Access Token (PAT), cloning the repo locally, committing changes, and pushing them back — a full workflow from local → cloud.

⚙️ Tools & Services Used

Azure DevOps Repos

Git Bash

Personal Access Token (PAT)

Windows 10

🪜 Steps Executed
🔹 Step 1 — Create Azure DevOps Repository

Logged into https://dev.azure.com

Opened project: AravindAzureLab

Navigated to Repos → Files

Initialized the repository using Add README.md

Confirmed default branch: main

🔹 Step 2 — Copy Repository Clone URL

Clicked Clone

Selected HTTPS

Copied URL:

https://dev.azure.com/geedulaaravind/AravindAzureLab/_git/AravindAzureLab

🔹 Step 3 — Configure Git Locally

Installed Git and verified installation:

git --version


Created working directory:

mkdir AzureDevOpsProjects
cd AzureDevOpsProjects

🔹 Step 4 — Clone Azure DevOps Repository
git clone https://dev.azure.com/geedulaaravind/AravindAzureLab/_git/AravindAzureLab


During first push, created a Personal Access Token (PAT)

Scope: Code (Read & Write)

Entered PAT as password

Clone successful:

Cloning into 'AravindAzureLab'...
Receiving objects: 100%
Resolving deltas: 100%

🔹 Step 5 — Create & Commit a New File

Entered repo:

cd AravindAzureLab


Created a file:

echo "This is Task 2 test file" > task2.txt


Stage & commit:

git add .
git commit -m "Added task2.txt for DevOps Task 2"

🔹 Step 6 — Push to Azure DevOps
git push


Output:

To https://dev.azure.com/geedulaaravind/AravindAzureLab/_git/AravindAzureLab
main -> main


Verified file in Repos → Files.

✅ Outcome

Local Git integrated with Azure DevOps

Secure PAT authentication working

Verified push–pull workflow

Real-world DevOps Git cycle completed

📸 Proof of Completion

Screenshot of Git Bash push

Screenshot of Azure DevOps repo showing task2.txt





