
# 📦 Spring Boot Multipart File Upload (Sample)

A minimal and clean **Java Spring Boot** project that demonstrates how to upload files using **multipart/form-data** ✅  
Perfect as a reference repo for interviews, backend practice, or plugging into bigger projects.

---

## ✨ Features

- 📤 Upload single file via `multipart/form-data`
- 📦 Upload with metadata (DTO + file)
- ✅ Validations (size / empty file / content type)
- 🧾 Clear API responses + error handling
- 🧪 Ready for Postman / cURL testing
- 🧱 Clean code structure (controller → service → storage)

---

## 🧰 Tech Stack

- ☕ Java [17/21]
- 🌱 Spring Boot [version]
- 🔧 Maven / Gradle
- 📄 Lombok (optional)
- 🧪 JUnit (optional)

---

## 🗂️ Project Structure

```txt
src/main/java/...
├── controller/     # REST endpoints
├── service/        # business logic
├── storage/        # file saving logic (local/cloud)
├── dto/            # request/response models
└── exception/      # custom errors + handler

