#  Mesh Grid Network-on-Chip (NoC) 4x4 Simulation

This project simulates a **4×4 Mesh Grid Network-on-Chip (NoC)** topology to study packet routing, latency, and congestion behaviors. It models how data packets traverse through routers in a multi-core chip environment using efficient routing algorithms.

##  What is NoC?

**Network-on-Chip (NoC)** is a communication subsystem on a chip, enabling efficient data exchange between different modules/cores in a SoC (System on Chip). The mesh topology is one of the most commonly used NoC architectures due to its scalability and regular structure.

##  Project Overview

*  **Topology**: 4x4 Mesh Grid
*  **Routing**: Deterministic XY Routing Algorithm
*  **Traffic**: Random packet injection and movement
*  **Metrics Observed**:

  * Latency
  * Throughput
  * Congestion

##  Features

* Router design with input/output buffers
* Simulation of packet movement across routers
* Time-step based routing visualization
* Analysis of packet delivery timing and hops

##  Technologies Used

* C/C++ (Simulation Logic)
* Data Structures (Queues for buffering)
* Matrix/Grid Representation for topology

##  Sample Output Parameters

* Number of packets transmitted and received
* Average delay and hop count per packet
* Congestion patterns in the mesh

##  How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/mesh-noc-4x4.git
   cd mesh-noc-4x4
   ```

2. Compile the code:

   ```bash
   g++ main.cpp router.cpp -o mesh_sim
   ```

3. Run the simulation:

   ```bash
   ./mesh_sim
   ```

##  Future Improvements

* Support for different topologies (e.g., torus, butterfly)
* Adaptive routing algorithms
* Graphical UI for simulation visualization
* Injection rate and fault modeling

## 🙌 Acknowledgements

Developed as part of coursework/project on **Computer Architecture / Network-on-Chip Systems**.

