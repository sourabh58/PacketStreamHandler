# PacketStreamHandler

This repository contains a C# program that demonstrates how to efficiently handle and process packet data received over a network stream. It's a practical example of a client application that communicates with a TCP server, retrieves streaming data, identifies missing packets, requests retransmissions, and assembles the complete dataset. The received data is then sorted and saved as a JSON file for further analysis.

Features:

- Establish a TCP connection with a server.
- Request and stream packets of data.
- Identify and request missing packets for retransmission.
- Assemble and sort received packets based on sequence.
- Generate JSON output of the assembled data for analysis.

## Prerequisites

Before running the program, ensure you have the following prerequisites installed on your machine:

- [.NET SDK](https://dotnet.microsoft.com/download/dotnet) for running C# programs.
- [Node.js](https://nodejs.org/) for running the TCP server.

## Getting Started

Follow these steps to reproduce the program on your machine:

1. Clone this repository to your local machine:

   ```bash
   git clone git@github.com:sourabh58/PacketStreamHandler.git

   ```

2. Navigate to the project directory:

   cd your-repo

Install the required Node.js dependencies for the TCP server. Run this command within the project directory:

    npm install

Start the TCP server. Run the following command within the project directory:

    node main.js

The server will start listening on port 3000.

3. Open Visual Studio Code or your preferred C# development environment and open the Program.cs file.

   - Modify the HOST and PORT variables in the Program.cs file to match the address and port where your TCP server is running.

   - Build and run the C# program using your development environment. The program will connect to the server and receive packets.

The program will create an output.json file in the project directory, containing the received packets in JSON format, sorted by sequence number.
