# Java Chat Application

This is a simple multi-threaded chat application developed in Java. It consists of two parts:
- *ChatServer*: A server that handles multiple client connections and facilitates message exchange.
- *ChatClient*: A client that allows users to connect to the server and participate in the chat.

## Features
- Allows multiple clients to connect simultaneously.
- Clients can send messages to the server, which broadcasts them to all connected clients.
- Clients can exit the chat by typing exit.
- Username validation to ensure only valid names are accepted.

## Project Structure

.
├── server
│   └── ChatServer.java
└── client
└── ChatClient.java

- server/ChatServer.java: Contains the implementation of the server, which listens for incoming connections and manages client threads.
- client/ChatClient.java: Contains the implementation of the client, which connects to the server and sends/receives messages.

## How to Run

### Prerequisites
- Java Development Kit (JDK) installed (version 8 or above)
- Basic knowledge of how to run Java programs from the command line

### Step 1: Compile the Code
Make sure you have both the ChatServer.java and ChatClient.java files saved in their respective directories. Open a terminal and navigate to the root directory of the project.

Compile the server and client code using the following commands:
```bash
# Compile the server
javac server/ChatServer.java

# Compile the client
javac client/ChatClient.java

Step 2: Run the Server

Start the server by running:

java server.ChatServer

You should see the following output:

Chat server is now active...

Step 3: Run the Client

In a new terminal window, run the client using:

java client.ChatClient

Upon running, the client will prompt for a username:

Please, enter your name:

Enter a valid username to join the chat. Once connected, the client can send and receive messages.

Step 4: Interact

	•	To send a message, type it and press Enter.
	•	To exit the chat, type exit and press Enter.

Example

	1.	Start the server:

Chat server is now active...


	2.	Start Client 1:

Please, enter your name: Alice
Welcome, [Alice] (ID: [1])! You have successfully connected to the chat.
Enjoy your time!


	3.	Start Client 2:

Please, enter your name: Bob
Welcome, [Bob] (ID: [2])! You have successfully connected to the chat.
Enjoy your time!


	4.	Client 1 types: Hello, everyone!
	•	Server output:

Alice: Hello, everyone!


	•	Client 2 sees:

Alice: Hello, everyone!



Notes

	•	Ensure that the server is running before starting any clients.
	•	The server and client currently run on localhost with port 12345. Update SERVER_ADDRESS and PORT in ChatClient.java if you want to change the server address or port.

License

This project is licensed under the MIT License - see the LICENSE file for details.

Contributions

Feel free to fork this project, raise issues, or make pull requests. All contributions are welcome!

Contact

For any questions, please reach out at [your-email@example.com].

Make sure to customize details like the LICENSE and Contact sections as needed. This README.md provides clear instructions on setting up and running your chat application, along with sample interactions to guide users.
