# Agentic-AI-Based-Smart-Course-Advising-System-for-Varsity


## 📌 Overview
This project presents an **Agentic AI-based Smart Course Advising System** for North South University (NSU). The system automates the traditional advising process using a **LangGraph-powered multi-agent workflow** and **LLM planning**, generating optimized, student-friendly course schedules.

---

## ❗ Problem Statement
The current advising system is:
- Manual or semi-automated  
- Time-consuming and inefficient  
- Lacks personalization  
- Unable to handle high demand vs limited seat availability  
- Prone to scheduling conflicts and unfair allocation  

---

## 💡 Proposed Solution
We designed an **Agentic AI system** that:
- Automatically assigns students to pre-advised courses  
- Ensures **seat availability constraints**  
- Maintains **strict theory-lab section matching**  
- Generates **optimized and healthy schedules**  
- Uses **multi-agent collaboration** for decision-making  

---

## 🤖 Agentic AI Workflow (Core Idea)

The system is built using a **LangGraph multi-agent architecture**, where each agent performs a specific task:

###  Agents Used

- **Advising Agent**
  - Selects course sections using LLM planning  
  - Ensures seat availability  
  - Maintains theory-lab pairing  

- **Days Evaluator Agent**
  - Minimizes number of class days (target: 4 days)  

- **Time Gap Evaluator Agent**
  - Optimizes time gaps between classes (ideal: ~90 mins)  

---

## 🔄 Workflow

1. **Input**
   - Pre-advising dataset (student course preferences)
   - Offered course dataset (sections, seats, timings)

2. **Advising Agent**
   - Selects valid sections using LLM reasoning
   - Checks:
     - Seat availability  
     - Theory-lab section matching  

3. **Evaluation Loop (LangGraph)**
   - Days Evaluator → checks total class days  
   - Time Gap Evaluator → checks schedule gaps  
   - If constraints fail → system retries with new section combinations  

4. **Final Output**
   - Conflict-free, optimized schedule  
   - Batch results for all students  

---

## ⚙️ Key Features

-  LangGraph Multi-Agent System  
-  LLM-Based Planning & Decision Making  
-  Seat-Aware Course Allocation  
-  Strict Theory-Lab Section Matching  
-  4-Day Routine Optimization (Flexible up to 6 days)  
-  Time Gap Optimization (90–180 mins)  
-  Iterative Feedback Loop for Optimization  
-  Batch Processing & Evaluation Output  

---

## 🏗️ System Architecture

