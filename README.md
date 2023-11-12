Creating a TCP server from scratch, even at its most basic level, involves several key capabilities:

1. **Socket Creation**: Establishing a socket is the first step in setting up a TCP server. This socket will listen for incoming TCP/IP connections.

2. **Binding to an Address**: The server must bind to an IP address and a port number so that clients know where to connect.

3. **Listening for Connections**: The server must listen on the bound address for incoming connection requests.

4. **Accepting Connections**: When a client attempts to connect, the server must accept the connection to establish communication.

5. **Handling Concurrent Connections**: Basic handling of multiple connections typically involves either handling one connection at a time in a sequential manner or managing multiple concurrent connections, possibly using threading or select/poll mechanisms.

6. **Receiving Data**: The server must be able to receive data sent by the client over the established connection.

7. **Sending Data**: Similarly, the server must be able to send data back to the client.

8. **Closing Connections**: After communication is complete, the server must properly close the connection.

9. **Error Handling**: Basic error handling for scenarios like network errors, client disconnections, and invalid data is necessary.

10. **Graceful Shutdown**: The server should be able to shut down gracefully, closing all active connections and releasing resources.

For robustness and scalability, further features such as secure connections (TLS/SSL), proper session management, and advanced error handling could be added after the basics are in place.