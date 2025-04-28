## CPU-Simulator GUI
A grahical user interface application with these components: CPU Simulator, QR code and Barcode Generator.


## Usage

```
Please install the font: "IDAutomationHC39M Free Version". You can find it in the project root folder.
```

## License
This project is licensed under the terms of the [MIT license](https://choosealicense.com/licenses/mit/).

# CPU Scheduling Simulator

[![GitHub](https://img.shields.io/badge/Repository-Link-blue)](https://github.com/carolinevarner/CPU-Simulator-GUI.git)

---

## Project Overview

This project is developed as part of CS 3502 - Operating Systems at Kennesaw State University.  
It simulates various CPU scheduling algorithms through a Windows Forms application.  
The project was originally forked from the starter code created by Francis Nweke and provided by Professor Chris Regan and has been **extended** by implementing additional algorithms for a complete evaluation.

---

## Project Instructions

### Introduction
As part of my Project 2 for Operating Systems, I simulated having a role at OwlTech Systems, a hypothetical company specializing in operating system optimization, and was tasked with evaluating different CPU scheduling algorithms.  
The company is concerned with **performance efficiency**, **fairness**, and **responsiveness** in process scheduling.

My responsibilities included:
- Analyzing the existing starter CPU scheduling simulator.
- Implementing new CPU scheduling algorithms beyond the basic ones provided.
- Measuring key performance metrics: average waiting time, turnaround time, and response time.
- Comparing the algorithms under various workload conditions.
- Documenting findings and recommending the best scheduling policy.

**Learning Outcomes:**
- Understanding and applying CPU scheduling techniques.
- Practical experience modifying/extending an existing codebase.
- Measuring and analyzing scheduling performance.
- Simulating real-world industry development practices.

### Starter Code Context
The starter project was located at:
> https://github.com/FrancisNweke/CPU-Simulator-GUI

The original algorithms included:
- First Come, First Served (FCFS)
- Shortest Job First (SJF)
- Round Robin (RR)
- Priority Scheduling

---

## Features and Changes

The extended project now supports **7 CPU scheduling algorithms**:

| Algorithm | Status | Description |
|:----------|:-------|:------------|
| FCFS | ✅ Starter Code | Schedules processes in the order they arrive. |
| SJF | ✅ Starter Code | Schedules the process with the shortest burst time first. |
| Priority Scheduling | ✅ Starter Code | Schedules based on process priority. |
| Round Robin (RR) | ✅ Starter Code | Cyclic scheduling with a fixed time quantum. |
| Shortest Remaining Time First (SRTF) | 🆕 **Added** | Preemptive scheduling based on the shortest remaining burst time. |
| Multi-Level Feedback Queue (MLFQ) | 🆕 **Added** | Processes move between multiple queues based on behavior. |
| Highest Response Ratio Next (HRRN) | 🆕 **Added** | Schedules process with the highest response ratio: (waiting time + burst time) / burst time. |

---

## Description of My Work

- **Forked** the original starter project into my GitHub account: [carolinevarner/CPU-Simulator-GUI](https://github.com/carolinevarner/CPU-Simulator-GUI).
- **Cloned** the repository locally using Visual Studio.
- **Added** three new scheduling algorithms (`SRTFAlgorithm`, `MLFQAlgorithm`, `HRRNAlgorithm`) inside `Algorithms.cs`.
- **Added** three new buttons to the GUI (`CpuScheduler.cs` and `Form1.cs`) for the new algorithms.
- **Followed** the original project structure and style using `Interaction.InputBox` and `MessageBox.Show`.
- **Maintained** the Windows Forms design style for seamless integration.
- **Tested** all algorithms under multiple process input scenarios.

---



## How to Run the Project

### Prerequisites
- Windows OS
- Visual Studio 2022 (or later)
- .NET Framework 4.7.2 or higher

---

### Setup and Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/carolinevarner/CPU-Simulator-GUI.git

2. Open the project in Visual Studio:
 - Open CpuSchedulingWinForms.sln.

3. Build and run:
 - Build Solution (Ctrl + Shift + B)
 - Run (F5)

4. Interact with the application:
 - Enter the number of processes.
 - Select an algorithm (including SRTF, MLFQ, HRRN).
 - Provide arrival and burst times as prompted.
 - View detailed results through popups and list views.

## **References**
 - Starter code: FrancisNweke/CPU-Simulator-GUI
 - CS 3502 Project 2: Operating Systems – CPU Scheduler Simulator Instructions

## **Contributors**  
- Francis Nweke (Starter Code)
- Caroline Varner
- Course: CS 3502 - Operating Systems 
- Instructor: Chris Regan
- University: Kennesaw State University
