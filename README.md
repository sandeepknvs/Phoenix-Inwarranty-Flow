   # 🚀 Postman API Automation Integration with GitHub Actions

This repository is a **Proof of Concept (POC)** that demonstrates how to integrate **Postman API tests with GitHub Actions** for continuous API testing.

The API tests are written in **Postman** and executed on a virtual machine using **Newman** and **newman-reporter-htmlextra**.  
GitHub Actions automatically triggers test execution on:

- Every push to the **main** branch  
- Manual execution using **workflow_dispatch**  
- Scheduled execution using **CRON jobs**

---

## 👨‍💻 About Me ##


Hi 👋 I’m Sandeep, a passionate Test Engineer / Aspiring SDET with hands-on experience in API Automation, CI/CD pipelines, and automation framework design.

I enjoy building end-to-end automation solutions, improving test reliability, and learning modern DevOps practices to strengthen QA engineering.

## You Can Contact me Here : https://www.linkedin.com/in/sandeepbolisetti/ ##




## 📌 Key Highlights

- Automated API test execution
- CI/CD integration using GitHub Actions
- HTML report generation using Newman
- Report hosting via GitHub Pages
- Email notification with latest test report
- Secure secrets management using GitHub Secrets

---

## 📊 Test Coverage

1. Happy Flow Testing  
2. Negative & Edge Case Testing  
3. Token-Based Authentication Testing  
4. Data-Driven Testing (CSV)  
5. JSON Schema Validation  
6. Secrets Management using GitHub Secrets  

---

## 📄 HTML Report

- The HTML report is generated inside the **Newman** folder.
- Reports are archived as **GitHub Action Artifacts**.
- The latest report is also hosted on **GitHub Pages**.

🔗 **Live Report:**  
https://sandeepknvs.github.io/Phoenix-Inwarranty-Flow/

![Postman Report](https://github.com/sandeepknvs/Phoenix-Inwarranty-Flow/blob/static-content/newman-report.PNG)

---

## 🧱 Project Structure

```text
Phoenix-Inwarranty-Flow
│
├── .github/
│   └── workflows/
│       └── postman-run.yml
│
├── newman/
│   └── index.html
│
├── Inwarranty-flow Collection.postman_collection.json
├── QA.postman_environment.json
├── TestData.csv
└── README.md
```


## 🛠️ Tech Stack

- Postman  
- Node.js (v22)  
- Newman  
- newman-reporter-htmlextra  
- GitHub Actions  
- GitHub Pages  
- Gmail SMTP  
- CSV (Data-Driven Testing)  
- AWS EC2 (Self-Hosted GitHub Runner)

---

## 🌐 GitHub Pages ##

You can directly view the **latest Postman test report** using GitHub Pages:

🔗 https://sandeepknvs.github.io/Phoenix-Inwarranty-Flow/

---

## How to Run the Project Locally ##

## Step 1: Clone the Repository ##

```
git clone https://github.com/sandeepknvs/Phoenix-Inwarranty-Flow.git

cd Phoenix-Inwarranty-Flow
```
## Step 2: Install Node.js and NPM ##
Download and install Node.js from the official website:
https://nodejs.org/en/download

Verify the installation:

```
node -v
npm -v
```

## Step 3: Install Newman ##

```
npm install -g newman
```
## Step 4: Install Newman HTML Extra Reporter

```
npm install -g newman-reporter-htmlextra
```

## Step 5: Execute the Postman Collection Using Newman ##

```
newman run "Inwarranty-flow Collection.postman_collection.json"
-e QA.postman_environment.json
-d TestData.csv
-r cli,htmlextra
```

## Step 6: View the HTML Report ##

```
./newman/index.html
```

## Note ##

Node.js version v18 or above is recommended

Ensure Postman collection, environment, and CSV files are present in the project root
---

## ⭐ Feedback & Contributions ##

Feedback and contributions are welcome.
If you find this project useful, feel free to ⭐ star the repository.




 
