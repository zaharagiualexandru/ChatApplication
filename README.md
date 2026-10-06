# 💬 Chat Application

**Chat Application** is a simple client/server messaging application built in **Unity / C#**.

The project allows one user to host a server while another user connects as a client using the server's **IP address**. Once connected, the two users can send messages to each other.

The project was created as an introduction to **network communication, client/server architecture and asynchronous application behaviour in C#**.

> Built with Unity and C#.

---

## 💬 How It Works

When the application starts, the user can choose to either:

- 🖥️ **Start Server**
- 💻 **Start Client**

If starting a client, the user enters the IP address of the machine running the server.

```text
Server
   │
   │  IP Address
   │
   ↓
Client
```

Once the connection has been established, the server and client can exchange messages through the chat interface.

Both machines need to be able to communicate over the same network/IP connection.

---

## 🕹️ Application Flow

```text
Launch Application
        ↓
Choose Server or Client
        ↓
 ┌───────────────┐
 │               │
Server          Client
 │               │
Start           Enter IP Address
 │               │
 └───────┬───────┘
         ↓
    Establish Connection
         ↓
      Chat Screen
         ↓
 Send / Receive Messages
```

---

## ✨ Features

- Client/server architecture
- IP-based connection
- Server hosting
- Client connection
- Two-way messaging
- Chat interface
- Connection management
- Separate client and server behaviour
- Unity UI
- C# networking logic

---

## 🧠 Client / Server Architecture

The application separates networking responsibilities between a **server** and a **client**.

### 🖥️ Server

The server acts as the host of the connection.

Once started, it waits for a client to connect.

After a connection has been established, the server can send and receive messages.

### 💻 Client

The client connects to the server using its IP address.

Once connected, it can communicate with the server through the chat interface.

This creates a simple architecture similar to:

```text
┌──────────────┐
│    SERVER    │
│              │
│ Send Message │
│ Receive      │
└──────┬───────┘
       │
       │ Network Connection
       │
┌──────▼───────┐
│    CLIENT    │
│              │
│ Send Message │
│ Receive      │
└──────────────┘
```

---

## 🛠️ Systems Implemented

The project includes systems for:

- Starting a server
- Starting a client
- Entering a server IP address
- Establishing a network connection
- Sending messages
- Receiving messages
- Updating the chat interface
- Managing separate server and client behaviour
- Switching between application screens
- Handling networking alongside Unity's main thread

---

## 🖥️ User Interface

The application begins with a simple connection menu.

The user can:

```text
Enter IP Address...

[ Start Server ]

[ Start Client ]
```

A server user can start hosting the application, while a client enters the correct IP address before connecting.

Once connected, the application moves to the chat interface where messages can be exchanged.

---

## 📸 Screenshots

<p align="center">
  <img src="Images/ChatApplication.png" width="800" />
</p>

---

## 💻 Technologies Used

| Technology | Usage |
|---|---|
| **Unity** | Application and UI development |
| **C#** | Networking and application logic |
| **Unity UI** | Menus and chat interface |
| **Git / GitHub** | Version control |

---

## 🎯 What I Learned

This project gave me experience with concepts that are different from a traditional single-player Unity game.

In particular, I worked with:

- Client/server architecture
- Network communication
- IP-based connections
- Sending data between applications
- Separating client and server responsibilities
- Asynchronous application behaviour
- Updating Unity UI from networking systems
- Structuring a Unity project around networking rather than gameplay

The project helped me better understand the basic architecture behind applications where multiple machines need to communicate with each other.

---

## 📦 Running the Project

To open the project locally:

1. Clone this repository.
2. Open **Unity Hub**.
3. Select **Add project from disk**.
4. Select the cloned `ChatApplication` folder.
5. Open the project.
6. Open the main `ChatAppScene`.
7. Press **Play**.

To test communication between two machines:

1. Start the application as the **Server** on one machine.
2. Find the IP address of the server machine.
3. Open the application on another machine.
4. Enter the server's IP address.
5. Select **Start Client**.
6. Once connected, both sides can exchange messages.

---

## 📌 Project Status

**Completed**

This project was developed as a networking-focused Unity project and is preserved as part of my programming portfolio.

---

## 👤 Developer

**Alex**

Games Programmer based in London.

🎮 Unity / C#  
⚙️ Unreal Engine 5 / C++  
🕹️ Gameplay Programming  
🛠️ Git / GitHub  
🧊 Blender  

[GitHub Profile](https://github.com/zaharagiualexandru)  
[itch.io](https://alexziou.itch.io/)  
[LinkedIn](YOUR-LINKEDIN-LINK)
