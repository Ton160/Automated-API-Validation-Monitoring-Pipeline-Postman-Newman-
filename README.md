# 🚀 Automated API Testing & Monitoring Pipeline (Postman + Newman)

## 🧠 Overview
This project demonstrates how API testing can be transformed into an automated and continuous validation process using Postman and Newman.

It simulates a real-world business use case where backend APIs are tested, validated, and monitored automatically to ensure system reliability and reduce manual effort.

---

## ⚙️ What This Project Does

- Automates API testing for a full CRUD lifecycle
- Handles authentication dynamically using tokens
- Stores and reuses data between requests (CourseID)
- Validates responses (status code, body, performance)
- Enables execution via Newman for automation

---

## 🏗️ Architecture

- API Testing Tool: Postman  
- Automation Runner: Newman  
- Environment Management: Postman Environment Variables  
- Execution Mode: CLI / CI-ready  

---

## 🔄 Workflow Scenario

This project simulates a complete business flow:

1. 🔐 **Login**
   - Authenticates user
   - Extracts token automatically
   - Stores it for future requests

2. ➕ **Create Course**
   - Sends POST request
   - Extracts Course ID dynamically

3. 🔍 **Get Course**
   - Validates:
     - Status code (200)
     - Response contains expected data
     - Response time (<200ms)

4. ✏️ **Update Course**
   - Updates course data (Java → Python)

5. ❌ **Delete Course**
   - Removes the course

6. 📋 **Get All Courses**
   - Validates overall API health

---

## 🧪 Test Coverage

- ✅ Status Code Validation (200, 201)
- ✅ Response Body Validation
- ✅ Dynamic Data Handling (Token & CourseID)
- ✅ Response Time Validation
- ✅ End-to-End API Flow Testing

---

## 💡 Key Features

- Dynamic authentication handling
- Data-driven testing using environment variables
- End-to-end API lifecycle validation
- Reusable and scalable test structure
- CLI execution using Newman
- Ready for CI/CD integration

---

## 🛠️ Tech Stack

- Postman  
- Newman  
- JavaScript (Postman Test Scripts)  

---

## 📂 Project Files

- `collection.json` → API test collection  
- `environment.json` → environment variables  
- `reports/` → Newman execution reports  

---

## ▶️ How to Run

### Run using Postman:
1. Import `collection.json`
2. Import `environment.json`
3. Select environment
4. Click **Run Collection**

---

### Run using Newman (CLI):

```bash
newman run collection.json -e environment.json -r html


###🎯 Business Value

This project represents how API testing can contribute to business transformation:

🔹 Reduces manual testing effort
🔹 Detects issues early in the pipeline
🔹 Improves system reliability
🔹 Enables continuous testing and monitoring
🔹 Supports faster and safer releases

##👨‍💻 Author

Antonious
Automation Testing & Business Transformation Enthusiast
