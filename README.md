# 23071A3232-OS-5
OS Unix Domain and Internet Domain Chat Applications
Chat Application using UNIX & Internet Domain Sockets

This repository contains two implementations of a simple chat application using IPC sockets:

    UNIX Domain Sockets (AF_UNIX) → For local inter-process communication.
    Internet Domain Sockets (AF_INET) → For communication over LAN/internet.

Overview
1️ UNIX Domain Sockets (AF_UNIX)

Used for: Local IPC (Inter-Process Communication) on the same system.
How it works: Uses a file path (/tmp/chat_socket) for communication.
Running the UNIX Domain Chat
Compile the server and client

gcc -o chat_server chat_server.c
gcc -o chat_client chat_client.c

This chat system follows a client-server model, where:

    The server listens for incoming connections.
    The client connects to the server and exchanges messages.

    Run the server in one terminal

    ./chat_server

Run the client in another terminal

./chat_client

    Start Chatting

    Type a message in the client, and it appears on the server.
    Type a message in the server, and it appears on the client.
    Type "exit" to close the chat.

2️ Internet Domain Sockets (AF_INET)

Used for: Local IPC (Inter-Process Communication) on the same system.
How it works: Uses a file path (/tmp/chat_socket) for communication.
Running the Internet Domain Chat
Compile the server and client

gcc -o chat_server_int chat_server_int.c
gcc -o chat_client_int chat_client_int.c

This chat system follows a client-server model, where:

    The server listens for incoming connections.
    The client connects to the server and exchanges messages.

    Run the server in one terminal

    ./chat_server_int

Run the client in another terminal

./chat_client_int

    Start Chatting

    Type a message in the client, and it appears on the server.
    Type a message in the server, and it appears on the client.
    Type "exit" to close the chat.

Contributors

    MALLUPEDDI VAMSI KRISHNA
    NISHANTH ROY KEERTHI
    KOLLA VIVEK SAGAR
    MALLIALA SRINIVAS
