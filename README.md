# 📂 Spring Batch with Directory Watcher

This Spring Boot application integrates **Spring Batch** with a **directory watcher** to monitor a folder for file changes (create, modify, delete) and automatically trigger batch jobs. Ideal for automating file-based ETL or processing pipelines.

---

## 🚀 Features

- ✅ Watches a target directory for file events
- ✅ Triggers Spring Batch jobs on new file creation
- ✅ Uses Java's built-in `WatchService`
- ✅ Modular structure with service and batch layers
- ✅ Configurable file path
- ✅ Clean and event-driven design

---

## 🏗️ Tech Stack

- Java 17+
- Spring Boot
- Spring Batch
- Java NIO WatchService
- Maven

---

▶️ How It Works
The app starts and initializes a background thread to watch the directory.

When a new file is created, the app detects the event.

A Spring Batch job is triggered to process the file.

The job can read, process, and write data as defined in batch config.

🧪 Running Locally

git clone https://github.com/jvcataquiz/SpringBatchWithDirectoryWatcher.git
cd spring-batch-directory-watcher-main
mvn spring-boot:run

📌 Use Cases
Automated CSV/Excel processing

Log file monitoring

File-based data import/export

Real-time batch job triggering