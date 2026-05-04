# 🗂️ Customised Virtual File System (CVFS)

### (C++ | System Programming | Mini OS Simulation)

## 📌 Description

The **Customised Virtual File System (CVFS)** is a system-level project written in C++ that simulates how an operating system manages files internally.

It recreates core OS components such as:

* Superblock
* Inodes
* File Table
* User File Descriptor Table (UFDT)

This project acts like a **mini file system shell**, allowing users to create, read, write, and manage files in memory.

---

## 🚀 Features

* 📁 Create virtual files (`creat`)
* 🗑️ Delete files (`unlink`)
* 📋 List files (`ls`)
* 📊 Display file info (`stat`)
* ✍️ Write data into file (`write`)
* 📖 Read data from file (`read`)
* 📖 Command help system (`man`, `help`)
* 🖥️ Custom interactive shell

---

## 🛠️ Technologies Used

* Language: **C++**
* Concepts:

  * File System Design
  * Inode-based architecture
  * Memory management
  * Linked list (DILB – Disk Inode List Block)
  * Command-line interface

---

## 🧠 Core Architecture

### 🔹 Superblock

* Tracks total and free inodes

### 🔹 Inode Structure

Each file is represented using an inode containing:

* File name
* File size
* File type
* Permissions
* Buffer (actual data)

---

### 🔹 File Table (UFDT)

* Maintains opened files
* Tracks read/write offsets

---

### 🔹 DILB (Disk Inode List Block)

* Linked list of all inodes
* Initialized at startup

---

## ⚙️ How It Works

1. System initializes:

   * BootBlock
   * SuperBlock
   * DILB
   * UAREA

2. User interacts via shell:

```bash
My CVFS >
```

3. Commands are parsed and executed:

* File operations handled using in-memory structures
* No real OS files are used

---

## 🧑‍💻 How to Run

### 🔧 Compile

```bash
g++ CVFS.cpp -o cvfs
```

### ▶️ Run

```bash
./cvfs
```

---

## 📂 Sample Commands

```bash
creat Demo.txt 3
write 0
read 0 10
ls
stat Demo.txt
unlink Demo.txt
help
exit
```

---

## 📊 Sample Output

```bash
My CVFS > creat Demo.txt 3
File is successfully created with FD : 0

My CVFS > write 0
Please enter the data...
10 bytes gets successfully written into the file

My CVFS > read 0 10
Data from file is : HelloWorld
```

---

## ⚠️ Limitations

* In-memory file system (no persistent storage)
* Limited number of files (MAXINODE = 5)
* Fixed file size (100 bytes)
* No directory structure

---

## 📈 Future Improvements

* Add persistent storage (save to disk)
* Add directory support
* Add file permissions (user/group)
* Add encryption
* Add GUI interface
* Add multi-user support

---

## 💡 Learning Outcomes

* Deep understanding of file systems
* OS internal concepts (inode, superblock)
* Memory-based data management
* Command interpreter design
* System-level programming

---

## 👤 Author

**Kartik Ganesh Jare**

---

## 📜 License

All Rights Reserved © 2026

---

## ⭐ Why This Project Matters

This is a **mini operating system–level project**.

It demonstrates:

* File system design
* OS-level thinking
* Data structure + system integration

👉 Extremely valuable for:

* System Programming roles
* OS interviews
* Product-based companies

---
