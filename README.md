# IoT Course Notes — Sapienza University (2024/2025)

> Concise study notes for the **Internet of Things (IoT)** course by **Prof. Viviana Arrigoni** (Department of Computer Science).  
> **This repository does not replace the official lecture PDFs**. It’s a streamlined companion for review and quick reference.

---

## Why this repo?

- **Fast revision:** condensed concepts, definitions, and diagrams.
- **Clear structure:** each chapter mirrors the official syllabus.
- **Bilingual content:** most notes provide **IT + EN** side by side (where relevant).
- **Open to fixes:** typos, clarifications, and small improvements via Issues/PRs.

---

## Contents

- **[1. Introduction](markdown/1-Introduction.md)** — *What IoT is and why it matters.*  
  Covers the basic definition (**IoT = Sensors + Networks + Data + Services**), the distinction between **IT** (secure connectivity among servers, DBs, apps) and **OT** (industrial operations with sensors/devices), and an overview of **Smart Objects** (sensing, compute, communication, actuation) with their core components (sensors, processing unit, memory, actuators, communication unit, power source). Introduces the idea of recurring **IoT architectures** and ubiquitous computing.


 - **[2. IoT Architecture](markdown/2-IoTArch.md)** — *Layers, classifications, and communication types.*  
  Explains the three main layers (**Sensor/Perception**, **Gateway/Network**, **Application/Analytics**), their functions, and device classifications (e.g., power source, mobility, reporting frequency, data richness, sensing/transmission range).  
  Details **M2M communication** and the main **network types** (PAN, HAN, NAN, FAN, LAN, LPWAN, Cellular), along with common **topologies** (Star, Clustered Star, Mesh, Tree).  
  Introduces the role of **Gateways** vs **Routers**, and the distribution of compute between **Edge, Fog, and Cloud**. Includes an example of **Fall Detection** optimisation problem (task offloading, cost minimisation, NP-complete nature).


  - **[3. IoT Devices](markdown/3-Devices.md)**
    — *Sensors and actuators in IoT systems.*  
    Introduces the role of **sensors** (transducers that convert physical signals into electrical ones) and their main types (e.g., accelerometers, gyroscopes, gas, humidity, touch, load cells, temperature).  
    Explains the concept of **ideal vs real sensors** (sensitivity, noise, non-linearity, bandwidth) and models of response.  
    Presents **actuators** as components that act on the environment, describing their motion (linear/rotary) and main energy sources (hydraulic, pneumatic, electric, thermal, magnetic).

---


## Author

**Andrea Maggiore** (Matricola: 1947898)