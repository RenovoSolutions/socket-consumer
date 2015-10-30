# socket-consumer
A simple browser application that connects to the socket server and displays the messages pushed through the socket.

# Overview
To see this demonstration working end to end:

* Clone and run the socket-source repository
   
`node index.js -c test -m "Test message"`

This will generate the exchange on the rabbit server, configuring it to be durable.

* Clone and run the socket-server repository

`node index.js -p 8002`

Set the port to whatever you like but make sure there are no conflicts.

* Clone the socket-client and serve the page via live-server, http-server, etc
* Launch a browser and point it to the index page (by default at http://localhost:8080/)
* Enter the port and a channel into the browser and click "Connect"
* In the socket-source app folder, run the node application and specify the channel you entered in the browser and a message
* You should see the message displayed in the browser. :tada:
