# console-project-network
# Console Connection Network - Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates how to configure a network device (Switch) using a **console connection** in Cisco Packet Tracer.

It focuses on basic device access and initial configuration through a direct connection between a PC and a Switch.

---

## 🧩 Network Topology

* 1 Switch
* 1 PC
* Console Cable (RS232 → Console Port)

---

## ⚙️ Configuration Steps

### 🔹 1. Connect Devices

* Connect the PC to the Switch using a **console cable**.

### 🔹 2. Access the Switch

* Open the PC
* Go to:

  ```
  Desktop → Terminal
  ```
* Press Enter to access CLI

---

### 🔹 3. Enter Privileged Mode

```
enable
```

---

### 🔹 4. Enter Global Configuration Mode

```
configure terminal
```

---

### 🔹 5. Configure Console Password

```
line console 0
password 1234
login
```

---

### 🔹 6. Set Enable Secret Password

```
enable secret 5678
```

---

### 🔹 7. Set Hostname

```
hostname SW1
```

---

### 🔹 8. Save Configuration

```
write memory
```

---

## 🔐 Security Notes

* `enable secret` is encrypted and more secure than `enable password`
* Always use `login` under console line to enforce password authentication

---

## 🎯 Learning Objectives

* Understand console access to network devices
* Learn basic Cisco CLI commands
* Configure passwords for secure access
* Navigate between different CLI modes

---

## 📁 File Included

* `console-project-network.pkt`

---

## 🚀 Author

Basmala Salah

---

## 💡 Notes

This is a beginner-level project for learning Cisco networking basics using Packet Tracer.
