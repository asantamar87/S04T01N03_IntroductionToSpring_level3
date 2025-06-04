# 📬 Postman Testing - Level 3 Exercise

In this level, you'll test your Spring Boot applications (created in Level 1 & Level 2) using **Postman**.

You'll learn how to use Postman environments and variables to dynamically send requests to different local servers.

---

## 🌐 Environments Setup

Create **two Postman environments**:

### 🔧 Maven Project Environment

| Variable | Value               |
|----------|---------------------|
| `servidor` | `http://localhost` |
| `port`     | `9000`             |

---

### 🔧 Gradle Project Environment

| Variable | Value               |
|----------|---------------------|
| `servidor` | `http://localhost` |
| `port`     | `9001`             |

---

## ✅ How to Test

Use the following dynamic URL syntax in Postman:

{{servidor}}:{{port}}/HelloWorld?nom=YourName
{{servidor}}:{{port}}/HelloWorld2/YourName


Make sure:

- You run **each project from Eclipse** before sending requests.
- The correct environment is selected in Postman.
- You see the expected response:

Hola, YourName. Estàs executant un projecte Maven
Hola, YourName. Estàs executant un projecte Gradle


---

## 📎 Deliverables

You must include the following 4 files in your Git repository:

- ✅ `maven-environment.json` (Exported from Postman)
- ✅ `gradle-environment.json` (Exported from Postman)
- 🖼️ Screenshot: Maven environment request using variables
- 🖼️ Screenshot: Gradle environment request using variables

Example screenshot content:

POSTMAN View:
✔️ Environment selected
✔️ URL using {{servidor}} and {{port}}
✔️ Response from Spring Boot app


---

## 🧪 Suggested Test URLs

```http
{{servidor}}:{{port}}/HelloWorld
{{servidor}}:{{port}}/HelloWorld?nom=John
{{servidor}}:{{port}}/HelloWorld2
{{servidor}}:{{port}}/HelloWorld2/John

📚 Additional Learning Resources

These references were useful in completing this task:

    📘 How to Use Postman Environments

    📘 Spring Boot REST API Testing with Postman