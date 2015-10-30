# socket-consumer
A simple browser application that connects to the socket server and displays the messages pushed through the socket.

# Overview
To see this demonstration working end to end:

1. Clone and run the socket-source repository
   `node index.js -c test -m "Test message"`
   This will generate the exchange on the rabbit server, configuring it to be durable.
2. Clone and run the socket-server repository
   `node index.js -p 8002`
   Set the port to whatever you like but make sure there are no conflicts.
3. Clone the socket-client and serve the page via live-server, http-server, etc
4. Launch a browser and point it to the index page (by default at http://localhost:8080/)
5. Enter the port and a channel into the browser and click "Connect"
6. In the socket-source app folder, run the node application and specify the channel you entered in the browser and a message
7. You should see the message displayed in the browser. :tada:
