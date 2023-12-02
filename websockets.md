## HTTP Protocol

- Unidirectional protocol where the client sends a request and the server responds.
- Utilizes a request-response model where each request corresponds to a single response.
- **Stateless** nature: Each request is independent and does not retain information from previous requests.
- Runs on top of TCP, a connection-oriented protocol ensuring reliable data delivery.
- Establishes a new TCP connection for each HTTP request and closes it after receiving a response.
- HTTP message information is encoded in ASCII.
- Message includes protocol version (HTTP/1.1, HTTP/2), methods (GET, POST), headers (Content-Type, Length), host information, and a body containing the message being transferred.
- Header sizes typically range from 200 bytes to 2 KB, with a common size of 700 - 800 bytes. Usage of more cookies and client-side tools may affect header payload size.

## Web Sockets

- WebSocket is a bidirectional, full-duplex communication protocol.
- It operates in the same client-server communication scenario as HTTP, but starts with `ws://` or `ws://` for secure connections.
- Unlike HTTP, WebSocket maintains a **stateful** connection between client and server until it's terminated by either party.
- After initiating the TCP connection through handshaking, a persistent connection is established between the client and server.
- This persistent connection, known as WebSocket, allows ongoing communication between client and server using the same connection channel.
- Message exchange occurs in a bidirectional mode as long as the connection persists.
- When either the client or server decides to close the connection, it is terminated by both parties.
- WebSocket's protocol switch is denoted by the **status code 101**, indicating the transition from HTTP to WebSocket.
