# Chatroom Application

## **Overview**

This project implements a simple chatroom application using socket programming in C. It consists of a Server and a Client program that facilitate real-time communication between multiple clients.

**Features**

Multiple clients can join the chatroom simultaneously.

Clients can send and receive messages in real-time.

Supports client disconnection handling.

Threaded implementation for handling multiple clients.

Graceful shutdown with Ctrl+C support.

**Getting Started**

**Compilation**

1. Clone the repository:
'''
git clone <repository_url>
cd <repository_name>
'''
2. Compile the Server:
'''
gcc -pthread server.c -o server
'''
3. Compile the Client:
'''
gcc client.c -o client
'''
**Usage**

**Start the Server**

Run the server on a specified port:
'''
./server <port>
'''
Example:
'''
./server 8080
'''
**Start the Client**

Run the client and connect to the server:
'''
./client <port>
'''
Example:
'''
./client 8080
'''
Enter your name when prompted and start chatting!

**Exiting the Chatroom**

Clients can type exit to leave the chatroom.

Use Ctrl+C to terminate the server.

**Example Interaction**

Start the server on a port:
'''
./server 8080
'''
Start multiple clients:
'''
./client 8080
'''
Clients can chat in real-time. Example:

Client 1: Hello!

Client 2: Hi there!

Output on Server:
'''
=== WELCOME TO THE CHATROOM ===
Client1 has joined
Client2 has joined
Hello! -> Client1
Hi there! -> Client2
'''
**Known Limitations**

The server runs on localhost (127.0.0.1) only. For remote connections, modify the IP in the server and client code.

No encryption or secure communication is implemented.
