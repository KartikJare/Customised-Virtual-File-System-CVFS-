# 🗂️ Customised Virtual File System (CVFS)

### (C / C++ | System Programming Project)

## 📌 Description

**Customised Virtual File System (CVFS)** is a system-level project that simulates a virtual file system inside a single application.

It demonstrates how operating systems manage files internally using concepts like:

* File tables
* Inodes
* File descriptors
* File metadata
* Read / write operations

---

## 🚀 Features

* 📁 Create virtual files
* 📖 Read file contents
* ✍️ Write data into files
* 🗑️ Delete files
* 📋 List available files
* 📊 Display file information
* 🧠 Simulates OS-level file management

---

## 🛠️ Technologies Used

* Language: **C / C++**
* Concepts:

  * Virtual File System
  * File Descriptor Table
  * Inode Management
  * File Handling
  * Memory Management
  * System Programming

---

## 📂 Project Structure

```bash
Customised-Virtual-File-System-CVFS-/
│── CVFS.c / CVFS.cpp
│── README.md
```

---

## ⚙️ How It Works

1. CVFS creates a virtual storage environment in memory
2. User can create, open, read, write, close, and delete files
3. File metadata is managed using inode-like structures
4. File operations are handled internally without directly depending on normal OS files

---

## 🧑‍💻 How to Run

### C

```bash
gcc CVFS.c -o CVFS
./CVFS
```

### C++

```bash
g++ CVFS.cpp -o CVFS
./CVFS
```

---

## 📌 Sample Commands

```bash
create Demo.txt 3
write Demo.txt
read Demo.txt 10
ls
stat Demo.txt
close Demo.txt
rm Demo.txt
exit
```

---

## 💡 Learning Outcomes

* Understanding internal working of file systems
* File descriptor and inode simulation
* System-level project design
* Memory-based file management
* OS concepts implementation

---

## 📈 Future Improvements

* Add persistent storage
* Add encryption support
* Add directory support
* Add user permissions
* Add GUI interface
* Add import/export functionality

---

## 👤 Author

**Kartik Ganesh Jare**

---

## ⭐ Why This Project Matters

This is a strong system-programming project because it shows how real operating systems manage files internally.

It is useful for:

* Operating System concepts
* System programming
* Low-level software development
* Interview and placement projects
