# 🐍 Python Server-Client Chat

This is a simple **Python socket project** that demonstrates a client-server chat system using TCP/IP.  
It allows a client to connect to a server, send messages, and safely disconnect using a special command.

---

## 📂 Project Structure

python-Server-Client/
│── server.py # Multi-threaded server code
│── client.py # Interactive client code
│── README.md # Documentation


---

## 🚀 Features
- Server handles multiple clients using **threading**
- Client sends messages to server using **TCP sockets**
- Fixed-size header (64 bytes) for message length
- Special command `!DISCONNECT` to close connection
- Safe workflow: server prints its IP & port; client uses them

---

## ⚙️ How to Run

### 1️⃣ Run the Server

```bash
python server.py


Server terminal will show:

[STARTING] Server is starting...
[LISTENING] Server is running on IP: 192.168.1.36 | PORT: 5050
Use this IP and PORT in your client.py to connect safely.

2️⃣ Update Client

Copy the IP and PORT from the server terminal into client.py:

SERVER = "127.0.0.1"  # Replace with server IP
PORT = 5050              # Replace with server PORT

3️⃣ Run the Client
python client.py


You can now type messages in the client terminal.

To exit, type:

!DISCONNECT

🔮 Future Improvements

Add multi-client broadcast for group chat

Add a GUI client (Tkinter or PyQt)

Add encryption for secure communication

Log message history

📖 Learning Goals

This project helped me learn:

Python socket programming

Client-server architecture

TCP communication

Multi-threading for handling multiple connections

👨‍💻 Author: Khush Rupapara
---
