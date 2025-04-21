# 22BCS15305_AbhayTiwari

# Java Chatting Application

A multi-user real-time chat application built with **Java Sockets** for networking and **Java Swing** for the graphical user interface.

## 🧠 Project Overview

This project demonstrates core Java concepts such as:
- Client-server communication using **TCP Sockets**
- **Multithreading** to handle concurrent users
- A responsive GUI using **Swing**
- Basic protocol for message exchange
- Dynamic user list updates
- Error handling for real-world network behavior

Developed as part of the **Bachelor of Engineering in Computer Science** curriculum at **Chandigarh University**.

## 👥 Authors

- **Abhay Tiwari** (22BCS15305)
- **Sujal Kumar** (22BCS17281)

## 📦 Features

- Connects multiple clients to a central server
- Real-time message broadcasting
- GUI with message area, input field, send button, and user list
- Displays online/offline status
- Handles both graceful and abrupt client disconnections
- Uses core Java only — no external libraries

## 🔧 Technologies Used

- Java (SE)
  - `java.net` for networking (Socket, ServerSocket)
  - `javax.swing` for GUI
  - `java.lang.Thread` for multithreading
  - `Collections.synchronizedSet` and `CopyOnWriteArraySet` for thread-safe data sharing

## 💻 How It Works

### Server
- Starts a `ServerSocket` on a configurable port
- For each incoming connection, spawns a new `ClientHandler` thread
- Handles message broadcasting and user list management

### Client
- Connects to the server using `Socket`
- GUI built with `JFrame`, `JTextArea`, `JTextField`, `JButton`, and `JList`
- A background thread listens for incoming messages and updates the GUI using `SwingUtilities.invokeLater`



