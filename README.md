# AntiProcrastinationApp
A Java-based Anti-Procrastination Task Manager with both CLI and GUI interfaces. Users can register/login, create tasks, mark them as completed, and track focus sessions using a Pomodoro-like timer. Data is saved to local files and presented via a clean and simple dashboard.


# ⏳ Anti-Procrastination Task Manager

A simple Java-based productivity tool to help users reduce procrastination and stay focused using task management and a built-in timer. Supports both CLI and GUI interfaces.

---

## 💡 Features

- 🧑‍💻 User registration and login
- ✅ Add and manage daily tasks
- 🎯 Start a Pomodoro-style focus timer
- 📊 View dashboard: total tasks, completed tasks, total focus time
- 💾 Data persistence using file system
- 🖥️ CLI and GUI available

---

## 🗂 Folder Structure
AntiProcrastinationApp/
│
├── model/                  ← Data classes (User, Task, TimerSession)
│   ├── User.java
│   ├── Task.java
│   └── TimerSession.java
│
├── service/                ← Logic: auth, file I/O, timer ops
│   ├── AuthService.java
│   ├── FileManager.java
│   └── TimerManager.java
│
├── ui/                     ← Swing GUI panels
│   ├── LoginPanel.java
│   ├── RegisterPanel.java
│   ├── DashboardPanel.java
│   ├── TimerPanel.java
│   └── TaskPanel.java
│
├── data/                   ← App data files (created at runtime)
│   ├── users.txt
│   ├── tasks.txt
│   └── sessions.txt
│
├── MainWindow.java         ← Main JFrame with CardLayout
├── AppLauncher.java        ← Main entry point (calls MainWindow)
└── README.md

---
Run CLI Version:
bash
java App
Run GUI Version:
bash
java ui.MainWindow
## 🚀 How to Compile

From the root directory:

```bash
javac -d . model/*.java service/*.java ui/*.java App.java
