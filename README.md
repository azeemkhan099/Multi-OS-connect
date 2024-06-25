# MultiOS Connect

MultiOS Connect is a cross-platform project designed to demonstrate communication between a Linux-based server and Windows-based clients. The server manages multiple clients simultaneously using threads, providing a robust example of inter-platform network programming.

## Features

- **Cross-Platform Communication**: Facilitates connection between a Linux server and Windows clients.
- **Multi-Client Handling**: The server can handle multiple clients concurrently using threading.
- **Socket Programming**: Utilizes socket programming to establish network communication.
- **Dynamic Interaction**: Clients send messages to the server, which responds appropriately.

## Table of Contents

- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Running the Server](#running-the-server)
- [Running the Client](#running-the-client)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Project Overview

This project demonstrates a basic client-server communication model where:
- The server (`server.c`) runs on a Linux machine, listens for incoming client connections, and handles each connection in a separate thread.
- The client (`client.c`) runs on a Windows machine, connects to the server, and exchanges messages with it.

### Server

- **Language**: C
- **Platform**: Linux
- **Functionality**: Listens on a specified port for incoming connections and spawns a new thread for each client.

### Client

- **Language**: C
- **Platform**: Windows
- **Functionality**: Connects to the server using its IP address and port, sends messages, and receives responses.

## Getting Started

To get started with MultiOS Connect, you will need a Linux machine for the server and a Windows machine for the client. Ensure you have the required tools installed on both systems.

### Prerequisites

- **Linux**: GCC compiler and POSIX threads library.
- **Windows**: Visual Studio (with C/C++ compiler) or MinGW for compiling the client code.

## Installation

Follow these steps to set up the project on your systems.

### Server Setup (Linux)

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/azeemkhan099/Multi-OS-connect
2. **Compile the Server Code:**
   gcc -o server server.c -lpthread
   
4. **Compile the Client Code:**
   gcc -o client.exe client.c -lws2_32
## Usage

**Start the Server:**
./server <number_of_tutors> <number_of_chairs>

**Start the Client:**
client.exe <IP-adress_of_server_network> <number_of_students> <number_of_help_session> <number_of_chairs>

