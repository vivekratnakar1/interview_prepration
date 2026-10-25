<div align="center">

# ☕ Java Interview Prep Hub

*A curated, high-impact collection of Core Java, Concurrency, Spring Boot, and System Design notes to ace your next backend engineering interview.*

[![Java Version](https://shields.io)](https://openjdk.org)
[![Spring Boot](https://shields.io)](https://spring.io)
[![Status](https://shields.io)]()
[![License](https://shields.io)]()

</div>

---

## 🚀 Overview

Welcome to my personal Java interview preparation vault. This repository is structured for quick revision, deep-dive architectural concepts, and high-frequency coding patterns asked in product-based and service-based companies.

---

## 📂 Repository Structure

| Module | Topics Covered | Status |
| :--- | :--- | :--- |
| **01-Core-Java** | OOPs, ClassLoaders, Exception Handling, String Pool, Reflection | `Completed` |
| **02-Collections-Generics** | `HashMap` internals, `ConcurrentHashMap`, Custom Comparators | `Completed` |
| **03-Multithreading** | Thread Lifecycle, `ExecutorService`, Locks, `CompletableFuture` | `In Progress` |
| **04-Modern-Java** | Lambdas, Stream API, Optional, Records (Java 17/21) | `Completed` |
| **05-JVM-Internals** | GC Algorithms, Heap vs Stack, JIT Compiler, Memory Leaks | `In Progress` |
| **06-Spring-Boot** | Dependency Injection, Scopes, AOP, Transactions, REST APIs | `Completed` |
| **07-Microservices** | Resilience4j, Kafka, Docker, Distributed Tracing | `Planned` |

---

## 🔥 High-Frequency Interview Questions

### Core Java & OOP
* **What is the difference between `==` and `.equals()`?**
  * `==` checks for reference (memory address) equality.
  * `.equals()` (when properly overridden) checks for value/state equality.
* **Explain Java's "Write Once, Run Anywhere" (WORA) principle.**
  * Java source code (`.java`) is compiled into platform-independent bytecode (`.class`), which is then interpreted/executed by the JVM specific to the host OS.

### Collections Framework
* **How does `HashMap` work internally?**
  * Uses hashing [hash() method], stores entries in an array of `Node<K,V>` buckets, and transitions from a linked list to a balanced Red-Black tree when bucket size exceeds threshold `TREEIFY_THRESHOLD = 8` (since Java 8).

### Modern Java (Streams & Lambdas)
```java
// Quick filter & map example using Java Streams
List<String> seniorDevs = engineers.stream()
    .filter(e -> e.getExperienceYears() >= 5)
    .map(Engineer::getName)
    .collect(Collectors.toList());
```

---

## ⚡ Quick Revision Cheatsheets

* [Core Java & OOP CheatSheet](./notes/core-java.md)
* [Concurrency & Threading Notes](./notes/concurrency.md)
* [Spring Boot & JPA FAQ](./notes/spring-boot.md)
* [SQL & Database Indexing Notes](./notes/sql-db.md)

---

## 🛠️ Tech Stack & Tools

* **Language:** Java 17 / Java 21
* **Framework:** Spring Boot 3
* **Build Tool:** Maven / Gradle
* **IDE:** IntelliJ IDEA Community / Ultimate

---

## 📈 Study Tracker / Roadmap

- [x] Revise OOP principles and Java memory model
- [x] Practice top 50 Collections & Concurrency scenarios
- [ ] Mock system design walkthrough for a URL shortener
- [ ] Solve 30 LeetCode Medium Java problems

---

## 🤝 Contributing / Feedback

Found an inaccurate explanation or want to add a killer interview question? Feel free to **Fork**, **Star ⭐**, or open a Pull Request!
