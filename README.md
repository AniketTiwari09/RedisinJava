# Redis Clone in Java

A simple Redis-like server implemented in Java, supporting basic `GET` and `SET` commands. Built to explore the fundamentals of key-value stores and server-client communication.

---

## Features

- Basic `GET` and `SET` command support.
- Multi-threaded client handling using Java Executors.
- Compatible with Redis CLI for testing.

---

## Getting Started

### Prerequisites
- Java JDK 18+
- Docker (optional, for benchmarking)

### Setup
1. **Clone the Repository**:
   ```
   git clone https://github.com/AniketTiwari09/RedisinJava.git
   cd RedisClone

2. Compile the Code:

   ```bash
    javac -d ./out src/RedisMain.java
  
3. Run the Server:

   ```bash
    java -cp ./out info.gamlor.redis.RedisMain

The server listens on 0.0.0.0:16381.

Test with Redis CLI:

     ```bash
      redis-cli -h 127.0.0.1 -p 16381
      SET key value
      GET key

Benchmarking
Run performance tests using Docker:

     ```bash
      docker run --name redisb --rm memtier_benchmark \
      --server=127.0.0.1 --port=16381 \
      -t 8 -c 32 --test-time=30 --pipeline=30

Author
Aniket Tiwari
GitHub: AniketTiwari09


### **Key Improvements:**
- Straightforward structure.
- Minimal instructions for quick setup and testing.
- Essential commands only.

Let me know if this works! 🚀
