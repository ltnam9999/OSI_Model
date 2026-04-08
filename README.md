# OSI_Model
This is a project I researched on my own to support my studies.
# 🌐 OSI Model — Research & Analysis

[cite_start]This repository contains research on the **OSI (Open Systems Interconnection)** model, focusing on stratified architecture and its 7-layer structure[cite: 1, 13].

## 📌 Overview
[cite_start]The OSI model is a reference framework developed by ISO in 1984 to describe how data is transmitted over a network by dividing the process into 7 independent layers[cite: 13].

## 📁 Table of Contents
* [🏗️ Stratified Architecture](#-stratified-architecture)
* [⚙️ Design Principles](#-design-principles)
* [🔄 Encapsulation Process](#-encapsulation-process)
* [📊 7-Tier Overview](#-7-tier-overview)
    * [Layer 7 - Application](#layer-7---application)
    * [Layer 4 - Transport](#layer-4---transport)
    * [Layer 3 - Network](#layer-3---network)
    * [Layer 1 - Physical](#layer-1---physical)

---

## 🏗️ Stratified Architecture
[cite_start]Layered architecture is a way of designing communication systems by dividing the process into independent layers[cite: 3]. [cite_start]It solves three core problems[cite: 5]:
* [cite_start]**Complexity:** Too complicated to manage[cite: 6].
* [cite_start]**Standards:** Lack of a common communication standard[cite: 7].
* [cite_start]**Maintenance:** Need for scalability and maintainability[cite: 8].

## ⚙️ Design Principles
* [cite_start]**Defined Functions:** Each floor performs a well-defined set of functions[cite: 15].
* [cite_start]**Neighbor Interaction:** Each floor only communicates with the adjacent upper and lower floors[cite: 16].
* [cite_start]**Independence:** Internal changes do not affect other layers as long as the interface remains constant[cite: 19].

## 🔄 Encapsulation Process
* [cite_start]**Encapsulation:** Data passes through all 7 layers top-down on the sending side[cite: 21, 22].
* [cite_start]**Decapsulation:** Data travels from the bottom up on the receiver side[cite: 21, 22].

## 📊 7-Tier Overview
| Layer | Name | Main Function | Data Unit |
| :--- | :--- | :--- | :--- |
| 7 | **Application** | [cite_start]Direct communication with user apps [cite: 26] | Data |
| 4 | **Transport** | [cite_start]End-to-end transmission & error control [cite: 26] | Segment |
| 3 | **Network** | [cite_start]Routing and logical addressing (IP) [cite: 26] | Packet |
| 2 | **Data Link** | [cite_start]Frame packing & MAC addressing [cite: 26] | Frame |
| 1 | **Physical** | [cite_start]Passing bits through physical environment [cite: 26] | Bit |

---
*Developed as part of personal research to support networking studies.*
