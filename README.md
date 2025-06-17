#  Mesh Grid Network-on-Chip (NoC) 4×4 Simulation

This project simulates a **4×4 Mesh Grid Network-on-Chip (NoC)** architecture, designed to analyze data communication within a multi-core processor system. It implements the **deterministic XY routing algorithm**, manages packet injection, and tracks performance metrics like **latency**, **throughput**, and **congestion**.

>  Ideal for learning NoC concepts, evaluating routing strategies, and simulating communication behavior in chip-level architectures.

---

## What is Network-on-Chip (NoC)?

In modern multi-core processors, traditional bus-based communication becomes a bottleneck. **Network-on-Chip (NoC)** addresses this issue by enabling high-bandwidth and scalable communication between processor cores, memory units, and other IP blocks through packet-switched networks.

A **mesh topology**, where routers are arranged in a grid-like structure, is widely used for its simplicity, scalability, and predictable performance.

---

## Project Highlights

| Feature              | Description                                                                       |
| -------------------- | --------------------------------------------------------------------------------- |
| **Topology**         | 4x4 Mesh Grid (16 nodes arranged in rows and columns)                             |
| **Routing**          | Deterministic XY Routing (always prioritizes horizontal, then vertical direction) |
| **Traffic Pattern**  | Randomized source-destination pairs for realistic load distribution               |
| **Clock Cycle Sim**  | Simulation proceeds in discrete time steps or clock cycles                        |
| **Performance Logs** | Logs number of hops, delays, and packet delivery success                          |

---

##  Core Features

*  **Buffered Routers**: Each node contains buffers for handling simultaneous packet flow.
*  **Discrete Time Simulation**: Progresses in steps, tracking packet movement at each clock cycle.
*  **Congestion Handling**: Identifies bottlenecks due to high packet traffic.
*  **Performance Metrics**:Latency (total time per packet), Hop count (number of routers visited), Packet drop count (if buffers overflow, if implemented), Router utilization

## Tech Stack

* **Language**: VERILOG
* **Concepts Used**:

  * OOP in C++ (classes for routers and packets)
  * Queue Data Structures
  * 2D Array for grid representation
  * Random Number Generation for traffic simulation


## Output Sample

The simulation provides detailed logs like:

```
Packet ID: 7
Source: (0,1)
Destination: (3,3)
Hops: 5
Total Delay: 9 cycles
---------------------------
Packet Delivered Successfully.
```

A summary report may also include:

* Total packets sent/received
* Avg. latency per packet
* Max buffer queue length
* Router congestion statistics

## How to Run

### Step 1: Clone Repository

```bash
git clone https://github.com/your-username/mesh-noc-4x4.git
cd mesh-noc-4x4
```

### Step 2: Compile Code

```bash
g++ main.cpp router.cpp -o mesh_sim
```

### Step 3: Run Simulation

```bash
./mesh_sim
```

## Future Enhancements

*  **Adaptive Routing Algorithms** (e.g., West-First, Turn Model)
*  **Fault Tolerance** for failed nodes or links
*  **Graphical Visualization** of packet flow and heatmaps
*  **Dynamic Traffic Models** based on real-world use-cases (multimedia, AI inference)
*  **Machine Learning-Based Routing** for intelligent traffic prediction

## Academic Relevance

This project is a part of the academic curriculum in **Computer Architecture / Advanced SoC Design**. It demonstrates real-world application of NoC systems, router modeling, and simulation-based performance evaluation.

> This simulation provides a practical learning experience in chip-level network communication, widely used in today’s multicore processors and embedded systems.


## Acknowledgements

This simulation was developed under the guidance of faculty in the **Department of Electronics and Communication / Computer Engineering** and is inspired by research and coursework related to Network-on-Chip systems.


