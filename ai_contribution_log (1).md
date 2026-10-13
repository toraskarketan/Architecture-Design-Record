# AI Contribution Log

**Course:** 02AML204 – Introduction to Artificial Intelligence  
**Student Name:** Ketan Gajanan Toraskar  
**Program:** SY B.Tech. CSE (AI & ML) | Semester VI  
**AI Collaboration Tool:** Gemini (Google)

---

## 📌 Overview

This contribution log documents the collaboration between the student (**Ketan Gajanan Toraskar**) and the AI assistant (**Gemini**) across the four Software Learning Experiences (SLEs). It details the prompt contexts, generated outputs, student modifications, and overall division of ownership to ensure academic integrity and transparency.

---

## 📅 SLE Breakdown & Contributions

### 1. SLE-1: Agent & Search Implementation
* **Task:** Building the initial 8-puzzle agent, defining search states, movement operators, and logging initial progress.
* **AI Contribution:**
  * Suggested clean code structure for state representation (3x3 matrix/array).
  * Provided template structure for logging AI interactions.
* **Student Contribution (Ketan):**
  * Wrote core movement validation logic (Up, Down, Left, Right).
  * Implemented initial search execution scripts and validated puzzle state constraints.
  * Documented initial setup in `README.md`.

---

### 2. SLE-2: Empirical Profiling & Performance Analysis
* **Task:** Profiling A* Search vs. Dijkstra’s Algorithm for solving the 8-puzzle problem.
* **AI Contribution:**
  * Provided code snippets for measuring execution time (`time`/`timeit`) and memory tracking during search.
  * Formatted profiling comparison tables (node expansions, execution time, path length).
* **Student Contribution (Ketan):**
  * Implemented the Manhattan Distance heuristic function.
  * Ran empirical test cases across various board difficulty configurations.
  * Collected and verified actual profiling data (node counts, memory overhead, runtime).
  * Analyzing trade-offs between unguided (Dijkstra) and guided (A*) search.

---

### 3. SLE-3: C4 Architecture Modeling
* **Task:** Designing system architecture diagrams using the C4 model framework (Context, Container, Component, Code).
* **AI Contribution:**
  * Drafted textual descriptions and component responsibilities based on C4 standards.
  * Suggested logical boundaries for breaking down the solver into modular containers (UI/CLI, Search Core, State Manager).
* **Student Contribution (Ketan):**
  * Designed and finalized C4 level 1, 2, 3, and 4 diagrams.
  * Mapped real Python code classes to individual component abstractions.
  * Verified architectural consistency between profiling components and model boundaries.

---

### 4. SLE-4: Architecture Decision Record (ADR) & Final Viva Defense
* **Task:** Authoring the ADR justifying the algorithm choice and preparing for oral viva defense.
* **AI Contribution:**
  * Structured the ADR according to the required SLE-4 template format (Context, Decision, Alternatives, Rationale, Consequences).
  * Generated viva preparation notes and questions based on course guidelines.
  * Assisted in drafting the GitHub repository `README.md`.
* **Student Contribution (Ketan):**
  * Selected the primary design decision (A* with Manhattan Distance over Dijkstra).
  * Injected empirical numbers from SLE-2 into the ADR rationale section.
  * Reviewed, edited, and approved all drafted content to align with actual project work.
  * Prepared personal verbal responses for oral viva questions.

---

## 📊 Summary of Ownership

| SLE | Metric / Task | AI Share (%) | Student Share (%) | Primary Student Responsibility |
| :--- | :--- | :---: | :---: | :--- |
| **SLE-1** | Code & State Setup | 30% | 70% | Core logic, movement constraints, execution |
| **SLE-2** | Profiling & Benchmarking | 25% | 75% | Running tests, heuristic logic, data collection |
| **SLE-3** | Architecture Modeling | 35% | 65% | Diagram creation, component mapping |
| **SLE-4** | ADR & Defense Prep | 30% | 70% | Rationale validation, ownership, viva defense |

---

## 🖋️ Student Declaration

I hereby declare that all technical implementations, data collection, architectural decisions, and final document submissions represent my own work. AI tools were utilized strictly for structural guidance, code optimization suggestions, and documentation formatting in accordance with course guidelines.

**Student Signature:** Ketan Gajanan Toraskar  
**Date:** October 14, 2026