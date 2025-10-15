# IoT Course Notes — Sapienza University (2024/2025)

> Concise study notes for the **Internet of Things (IoT)** course by **Prof. Viviana Arrigoni** (Department of Computer Science).  
> **This repository does not replace the official lecture PDFs**. It’s a streamlined companion for review and quick reference.

---

## Why this repo?

- **Fast revision:** condensed concepts, definitions, and diagrams.
- **Clear structure:** each chapter mirrors the official syllabus.
- **Bilingual content:** most notes provide side by side (where relevant).
- **Open to fixes:** typos, clarifications, and small improvements via Issues/PRs.

---

## Contents

- **[1. Introduction](markdown/1-Introduction.md)** — *What IoT is and why it matters.*  
  Covers the basic definition (**IoT = Sensors + Networks + Data + Services**), the distinction between **IT** (secure connectivity among servers, DBs, apps) and **OT** (industrial operations with sensors/devices), and an overview of **Smart Objects** (sensing, compute, communication, actuation) with their core components (sensors, processing unit, memory, actuators, communication unit, power source). Introduces the idea of recurring **IoT architectures** and ubiquitous computing.


 - **[2. IoT Architecture](markdown/2-IoTArch.md)** — *Layers, classifications, and communication types.*  
  Explains the three main layers (**Sensor/Perception**, **Gateway/Network**, **Application/Analytics**), their functions, and device classifications (e.g., power source, mobility, reporting frequency, data richness, sensing/transmission range).  
  Details **M2M communication** and the main **network types** (PAN, HAN, NAN, FAN, LAN, LPWAN, Cellular), along with common **topologies** (Star, Clustered Star, Mesh, Tree).  
  Introduces the role of **Gateways** vs **Routers**, and the distribution of compute between **Edge, Fog, and Cloud**. Includes an example of **Fall Detection** optimisation problem (task offloading, cost minimisation, NP-complete nature).


- **[3. IoT Devices](markdown/3-Devices.md)** — *Sensors, actuators, embedded systems, energy, and stochastic models.*
Covers sensors (types, ideal vs real, models) and actuators (motion, energy sources). Introduces embedded systems (MCUs, SoCs, Cortex-M, buses, memory, interrupts), with focus on cost/energy trade-offs, low-power modes, and optimisation strategies. Explains energy harvesting (sources, techniques, optimisation), and presents stochastic modelling tools: Markov Chains (transition matrices, stationary distributions, irreducibility, periodicity, Fundamental Theorem) and Markov Decision Processes (states, actions, policies, rewards, Bellman equations, optimality, dynamic programming, Q-learning).

- **[4. Information Theory](markdown/4-Information.md)** — *Entropy, binary encodings, mutual information, and communication channels.*  
Covers **entropy** as a measure of uncertainty (discrete and differential forms), **information content/surprisal**, and **binary entropy**. Introduces **binary encodings** of finite alphabets, with focus on variable-length, prefix-free and uniquely decodable codes. Explores **joint entropy** and **mutual information** to quantify dependencies between random variables. Describes **Discrete Memoryless Channels (DMC)** via transition probability matrices, including their role in modelling communication systems. Extends to **Gaussian channels**, presenting **differential entropy** and the **Shannon–Hartley theorem** for channel capacity as a function of bandwidth and signal-to-noise ratio (SNR).


- **[5. Communication](markdown/5-Communication.md)** — *Wireless communication, MAC protocols, and mesh networking.*  
Covers how IoT devices exchange data through **radio frequency communication**, explaining **antenna design**, **signal propagation**, **MIMO**, and **modulation schemes** (ASK, FSK, PSK, QAM) with their performance trade-offs. Describes **multiple access techniques** (TDMA, FDMA, ALOHA, CSMA/CA, CDMA) used to manage collisions and channel sharing. Introduces **power-saving mechanisms** and **MAC protocols** for wireless sensor networks (e.g., **S-MAC**, **TRAMA**). Concludes with **mesh networking**, addressing strategies (hardware, geographic, hierarchical) and major **routing algorithms** such as **OLSR**, **DSR**, **AODV**, and **Gossip Routing**, enabling scalable and energy-efficient IoT communication.


---


## Author

**Andrea Maggiore** (Matricola: 1947898)