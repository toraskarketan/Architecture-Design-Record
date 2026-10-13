# 8-Puzzle Solver: AI Search Profiling & Architecture Decision Record (ADR)

**Course:** 02AML204 – Introduction to Artificial Intelligence  
**Program:** SY B.Tech. CSE (AI & ML) | Semester VI  
**Student Name:** Ketan Gajanan Toraskar  

---

## 📌 Project Overview

This repository documents the end-to-end design, implementation, performance profiling, architecture modeling, and architectural justification for an **8-Puzzle AI Solver Agent**. The project spans across four distinct Software Learning Experiences (SLEs), bridging core artificial intelligence concepts with practical software engineering and architectural decision-making.

---

## 🚀 Learning Experience (SLE) Summary

### 🧩 SLE-1: Agent & Search Implementation
* Built the core state-space search engine for the 8-puzzle problem.
* Configured state representation, board movement validation, and transition logic.
* Maintained an **AI Contribution Log** and initial setup documentation.

### 📊 SLE-2: Empirical Profiling & Performance Analysis
* Evaluated informed search (**A* Search with Manhattan Distance**) against unguided search (**Dijkstra’s Algorithm**).
* Profiled key performance metrics:
  * Total node expansions
  * Execution time (milliseconds)
  * Peak memory usage (priority queue and closed list state retention)
  * Path cost and solution optimality

### 📐 SLE-3: C4 Architecture Modeling
* Designed the high-level system architecture using the **C4 Model** framework:
  * **Level 1 (Context Diagram):** User interaction with the search solver.
  * **Level 2 (Container Diagram):** Breakdown into UI/CLI Layer, Search Core Engine, and State Validation Service.
  * **Level 3 (Component Diagram):** Granular separation of Priority Queue, Heuristic Evaluator, and State Node Manager.
  * **Level 4 (Code Diagram):** Data structure and class relationships.

### 📝 SLE-4: Architecture Decision Record (ADR) & Defense
* Formally documented the critical design choice in an **Architecture Decision Record (ADR)**.
* Justified algorithm selection using empirical numbers from SLE-2 and container design principles from SLE-3.
* Prepared oral defense materials for viva evaluation.

---

## 🏛️ Architecture Decision Record (ADR)

* **Title:** Adoption of A\* Search with Manhattan Distance Heuristic over Dijkstra’s Algorithm
* **Status:** Accepted
* **Context:** Solving the 8-puzzle requires exploring a state space of up to $181,440$ reachable configurations. Uniform-cost approaches explore nodes blindly in all directions, causing heavy memory overhead.
* **Decision:** Selected **A\* Search** with the **Manhattan Distance heuristic** $f(n) = g(n) + h(n)$ as the primary search strategy.
* **Key Rationale:**
  * **70–80%+ Reduction in Node Expansions:** Manhattan distance guides search directionally toward the goal state.
  * **Optimality Guaranteed:** Manhattan distance is an admissible and consistent heuristic (never overestimates remaining step cost).
  * **Seamless C4 Integration:** Decouples heuristic calculations cleanly from state management components.

---

## 🛠️ Tech Stack & Concepts

* **Language:** Python 3.x
* **Algorithms:** A\* Search, Dijkstra's Algorithm / Uniform-Cost Search
* **Heuristics:** Manhattan Distance, Misplaced Tiles
* **Architecture:** C4 Model Framework
* **Profiling & Metrics:** Node expansion counters, time analysis (`time`/`timeit`), memory tracking

---

## 📋 File Structure

```text
.
├── src/
│   ├── main.py              # Main entry point / CLI interface
│   ├── search_engine.py     # Implementation of A* and Dijkstra algorithms
│   ├── heuristic.py         # Manhattan distance calculation logic
│   └── state_node.py        # 8-Puzzle board state representation
├── docs/
│   ├── SLE-1_Readme.md      # SLE-1 documentation & AI Log
│   ├── SLE-2_Profiling.pdf  # SLE-2 Empirical Profiling Report
│   ├── SLE-3_C4_Model.pdf   # SLE-3 C4 Architecture Diagrams
│   └── SLE-4_ADR.pdf        # SLE-4 Final Architecture Decision Record
└── README.md                # Project README file
```

---

## 👤 Author

* **Name:** Ketan Gajanan Toraskar
* **Course:** 02AML204 – Introduction to Artificial Intelligence
* **Department:** Computer Science & Engineering (AI & ML)