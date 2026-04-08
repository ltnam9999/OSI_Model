# OSI_Model
This is a project I researched on my own to support my studies.
# 🌐 OSI Model — Comprehensive Research & Analysis

This repository contains a full-scale research on the **OSI (Open Systems Interconnection)** model, covering its stratified architecture, design principles, and a detailed deep-dive into each of its 7 layers.

---

## 📁 Table of Contents
* [🏗️ Stratified Architecture](#-stratified-architecture)
* [❓ What is the OSI Model?](#-what-is-the-osi-model)
* [⚙️ Design Principles](#-design-principles)
* [🔄 Data Packaging (Encapsulation & Decapsulation)](#-data-packaging-encapsulation--decapsulation)
* [📊 7-Tier Overview Table](#-7-tier-overview-table)
* [🔍 Detailed Layer Operations](#-detailed-layer-operations)
    * [7. Application Layer](#7-application-layer)
    * [6. Presentation Layer](#6-presentation-layer)
    * [5. Session Layer](#5-session-layer)
    * [4. Transport Layer](#4-transport-layer)
    * [3. Network Layer](#3-network-layer)
    * [2. Data Link Layer](#2-data-link-layer)
    * [1. Physical Layer](#1-physical-layer)

---

## 🏗️ Stratified Architecture
Layered architecture in a network is a way of designing a communication system by dividing the entire communication process into many independent layers. Each floor assumes a clear role and only interacts with the layers adjacent to it.

Stratified architecture was born to solve three core problems:
* **Complexity:** Systems were too complicated to manage as a single unit.
* **Standardization:** There was no common standard for communication between different vendors.
* **Maintenance:** Layers allow the system to be expandable and maintainable.



[Image of OSI layered architecture model]


## ❓ What is the OSI Model?
The OSI (Open Systems Interconnection) model is a standard reference framework developed by the ISO (International Organization for Standardization) in 1984. This model describes how data is transmitted over a network by dividing the communication process into 7 separate layers.

## ⚙️ Design Principles
1. Each floor performs a well-defined set of functions.
2. Each floor only communicates with the adjacent upper and lower floors.
3. The number of floors is enough to group similar functions, but not so many that they become complex.
4. Boundaries between floors are defined to minimize the flow of information back and forth.
5. Each floor can be changed internally without affecting others, as long as the interface remains constant.

## 🔄 Data Packaging (Encapsulation & Decapsulation)
When an application sends data, it passes through all 7 layers in a **top-down** direction on the sending side (Encapsulation) and **bottom-up** on the receiver side (Decapsulation).

---

## 📊 7-Tier Overview Table

| Layer | Name | Main Functions | Data Unit | Protocols / Examples |
| :--- | :--- | :--- | :--- | :--- |
| 7 | **Application** | Direct communication with user apps | Data | HTTP, FTP, SMTP, DNS |
| 6 | **Presentation** | Format conversion, encryption, compression | Data | SSL/TLS, JPEG, MP3 |
| 5 | **Session** | Establish, maintain, and end sessions | Data | NetBIOS, RPC |
| 4 | **Transport** | End-to-end reliability, error control | Segment | TCP, UDP |
| 3 | **Network** | Routing, logical addressing (IP) | Packet | IP, ICMP, OSPF, BGP |
| 2 | **Data Link** | Frame packing, MAC addressing | Frame | Ethernet, ARP, PPP |
| 1 | **Physical** | Passing bits through physical environment | Bit | Cables, electrical signals |

---

## 🔍 Detailed Layer Operations

### 7. Application Layer
The highest layer and closest to the user. It provides network services directly to applications.
* **Key functions:** Identify communication partners, check resource availability, and synchronize communication.
* **Example:** When you enter `https://google.com`, the client creates a request: `GET /search?q=chatgpt HTTP/1.1`.

### 6. Presentation Layer
Responsible for translating data into a common format.
* **Main Functions:** Convert between character encoding standards (ASCII, EBCDIC, Unicode), data compression, and encryption.
* **Example:** Normalizing data so that Machine A (ASCII) can communicate with Machine B (EBCDIC) via UTF-8.

### 5. Session Layer
Manages the establishment, maintenance, and termination of sessions.
* **Functions:** Session ID management (e.g., staying logged into a website), Synchronization (checkpoints for large transfers), and Dialog control (Half-duplex/Full-duplex).

### 4. Transport Layer
The center of the OSI model, providing end-to-end reliable communication.
* **Functions:** Data segmentation (dividing large files into smaller segments) and reassembling at the receiving end.
* **Example:** Establishing a TCP connection via a three-way handshake (SYN -> SYN-ACK -> ACK).

### 3. Network Layer
Responsible for routing packets across various networks.
* **Functions:** Logical Addressing (IP), Routing (determining the optimal
