# CPU Scheduling Simulator

> An interactive web-based simulator for visualizing FCFS and Non-Preemptive SJF CPU scheduling algorithms with dynamic Gantt chart generation and performance metric evaluation.

---

## Table of Contents

* Overview
* Features
* Scheduling Algorithms
* Calculation Logic
* Technology Stack
* Project Structure
* File Structure Explanation
* Installation
* Usage
* Educational Objective
* Future Enhancements
* Live Demo

---

## Overview

This project is a frontend-based CPU Scheduling Simulator developed to demonstrate core operating system scheduling concepts through interactive visualization. Users can enter process details, select a scheduling algorithm, and simulate execution while observing computed performance metrics and graphical timelines.

The application focuses on clarity, correctness, and structured implementation suitable for academic submission.

---

## Features

* Dynamic addition of multiple processes
* Input fields for Process ID, Arrival Time, and Burst Time
* Algorithm selection (FCFS or Non-Preemptive SJF)
* Real-time CPU simulation
* Automatic shortest job selection (SJF Non-Preemptive)
* Graphical Gantt Chart representation
* Waiting Time calculation
* Turnaround Time calculation
* Average Waiting Time computation
* Input validation and error handling

---

## Scheduling Algorithms

### First Come First Serve (FCFS)

Processes execute strictly in order of arrival. This is a simple non-preemptive scheduling strategy.

### Shortest Job First (SJF) – Non-Preemptive

At every CPU decision point, the process with the shortest burst time among arrived processes is selected. Once execution begins, the process runs until completion.

---

## Calculation Logic

```
Waiting Time = Start Time − Arrival Time
Turnaround Time = Completion Time − Arrival Time
Average Waiting Time = Σ Waiting Time / Number of Processes
```

---

## Technology Stack

* React
* TypeScript
* Vite
* CSS

The application is implemented as a single-page frontend system without backend dependencies.

---

## Project Structure

```
.
├── index.html
├── package.json
├── tsconfig.json
├── vite.config.ts
├── src/
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
```

---


## Installation

Clone the repository:

```
git clone <repository-url>
cd <project-folder>
```

Install dependencies:

```
npm install
```

Run development server:

```
npm run dev
```

---

## Usage

1. Enter process details.
2. Select a scheduling algorithm.
3. Click "Simulate".
4. Observe the generated Gantt chart and computed metrics.

---

## Educational Objective

This project was developed as part of an academic assignment to demonstrate understanding of CPU scheduling mechanisms and performance evaluation metrics in operating systems.

---

## Future Enhancements

* Preemptive SJF implementation
* Round Robin scheduling
* Adjustable animation speed
* Exportable simulation reports
* Enhanced visualization refinements

---

## Live Demo

[https://fcfssjf-scheduling.vercel.app](https://fcfssjf-scheduling.vercel.app)
