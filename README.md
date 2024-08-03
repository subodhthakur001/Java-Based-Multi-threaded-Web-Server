# Multithreaded Web Server Project

## Overview

This project is a Java-based web server designed to compare the performance of single-threaded and multithreaded implementations, including a multithreaded server with a thread pool. The project includes separate implementations for each type of server, each with its own client.

## Project Structure

### Single-Threaded Server

- `singlethreaded/Server.java`: Implementation of a single-threaded web server.
- `singlethreaded/Client.java`: Client to interact with the single-threaded server.

### Multithreaded Server

- `multithreaded/Server.java`: Implementation of a multithreaded web server.
- `multithreaded/Client.java`: Client to interact with the multithreaded server.

### Thread Pool Server

- `threadpool/Server.java`: Implementation of a multithreaded web server with a thread pool.

## Getting Started

### Prerequisites

- Java Development Kit (JDK) 8 or higher
- Apache Maven (optional, for managing dependencies and building the project)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/multithreaded-web-server.git
    cd Java-Based-Multi-threaded-Web-Server
    ```

2. Compile the project:
    ```sh
    javac singlethreaded/*.java multithreaded/*.java threadpool/*.java
    ```

### Running the Servers and Clients

1. **Single-Threaded Server and Client**:
    - Start the single-threaded server:
        ```sh
        java singlethreaded.Server
        ```
    - Start the single-threaded client:
        ```sh
        java singlethreaded.Client
        ```

2. **Multithreaded Server and Client**:
    - Start the multithreaded server:
        ```sh
        java multithreaded.Server
        ```
    - Start the multithreaded client:
        ```sh
        java multithreaded.Client
        ```

3. **Thread Pool Server and Client**:
    - Start the thread pool server:
        ```sh
        java threadpool.Server
        ```
### Testing and Comparison

The project allows for performance testing and comparison of the different server implementations. You can run the clients to generate load and observe the behavior and performance metrics of each server type.

## Performance Comparison

### Single-Threaded Server

- Handles one request at a time.
- Simple but not efficient under heavy load.

### Multithreaded Server

- Utilizes multiple threads to handle requests simultaneously.
- Provides better performance and responsiveness compared to the single-threaded server.
- Can face resource exhaustion under extremely high loads.

### Thread Pool Server

- Uses a pool of threads to manage request handling.
- Limits the number of concurrent threads to prevent resource exhaustion.
- Provides a balance between performance and resource management.

## Contributing

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- Inspired by the need to understand and improve server performance.
- Special thanks to open-source community contributions and educational resources on multithreading and server design.

---

Feel free to reach out with any questions or feedback!
