# 🔥 BlazeCache

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](https://github.com/) [![Version](https://img.shields.io/badge/version-1.0.0-blue)](https://github.com/) [![License](https://img.shields.io/badge/license-MIT-orange)](https://github.com/)

A high-performance, in-memory caching server built from scratch with Node.js and TypeScript, using a raw TCP socket-based protocol for low-latency operations.

---

## Overview

BlazeCache is a learning project designed to explore the fundamentals of networking, concurrency, and systems programming within the Node.js ecosystem. Unlike traditional web applications that use HTTP, BlazeCache implements a custom, text-based protocol over TCP for maximum performance, similar to industry-standard tools like Redis and Memcached.

The core purpose of this project is to demonstrate a deep understanding of the Node.js event loop, asynchronous I/O, and the design of network protocols.

---

## Features

-   **In-Memory Storage**: All data is stored in RAM for microsecond-level read/write operations using a JavaScript `Map`.
-   **TCP Server**: Built using Node.js's native `net` module for a persistent, low-overhead connection between the client and server.
-   **Simple Text Protocol**: A human-readable, newline-delimited protocol for client-server communication.
-   **Concurrency Model**: Efficiently handles thousands of concurrent client connections on a single thread using the Node.js event loop.
-   **Typed with TypeScript**: The entire codebase is written in TypeScript for robust, maintainable, and scalable code.

---

## Tech Stack

-   **Language**: **TypeScript**
-   **Runtime**: **Node.js**
-   **Core APIs**:
    -   `net` module for TCP socket programming.
    -   `Buffer` module for handling raw binary data streams.

---

## Getting Started

Follow these instructions to get a local copy up and running.

### Prerequisites

Make sure you have the following installed on your machine:
-   Node.js (v18.x or later)
-   NPM or Yarn
-   `telnet` or a similar TCP client for testing.

### Installation

1.  Clone the repository:
    ```sh
    git clone [https://github.com/your-username/blazecache.git](https://github.com/your-username/blazecache.git)
    ```
2.  Navigate to the project directory:
    ```sh
    cd blazecache
    ```
3.  Install the dependencies:
    ```sh
    npm install
    ```

### Running the Server

To start the development server with hot-reloading:
```sh
npm run dev