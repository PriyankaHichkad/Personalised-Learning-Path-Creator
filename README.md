---
TITLE: Personalised-Learning-Path-Creator
AUTHOR: Priyanka Rajeev Hichkad
---

# AI-Powered Personalized Learning Path Generator

## Overview
This project demonstrates the development of an **AI Agent workflow using n8n** that automatically generates a structured and personalized learning path based on a user's input skill.

The workflow integrates **AI reasoning, web search, and task management tools** to create actionable learning steps and store them directly in a Notion database.

---

## n8n Workflow
![n8n](https://github.com/PriyankaHichkad/Personalised-Learning-Path-Creator/blob/main/n8n%20workflow%20on%20canvas.jpeg)

---

## Objective
The goal of this project is to:
- Automate the process of researching and structuring learning resources
- Eliminate manual effort in searching and organizing study plans
- Build a practical AI agent capable of **tool usage and workflow automation**

---

## Workflow Architecture
The workflow follows this pipeline:
Chat Trigger → AI Agent → (Search Tool + Notion Tool)

---

### Step-by-step Flow:
1. User inputs a skill (e.g., *Machine Learning*)
2. AI Agent processes the request
3. Uses **SerpAPI** to search relevant learning resources
4. Generates structured learning steps
5. Uses **Notion Tool** to create tasks in a database
6. Each step is stored with metadata like:
   - Task Name (sub-topic)
   - Status
   - Assignee
   - Priority
   - Due Date
   - Description
   - Effort Level

---

## AI Agent Design

The AI Agent is designed with:
- Controlled tool usage (search only once)
- Structured reasoning and planning
- Strict schema alignment with Notion database

### Tools Used:
- **Search Tool (SerpAPI)** → Fetch learning resources
- **Notion Tool** → Store structured tasks
- **Chat Model (OpenRouter)** → Reasoning and generation

---

## Technologies Used

- **n8n** – Workflow automation platform  
- **OpenRouter Chat Model** – AI reasoning engine  
- **SerpAPI** – Web search API  
- **Notion API** – Task management database  

---

## Key Features

- Automated research and summarization  
- Structured learning path generation  
- Task prioritization and effort estimation  
- Direct integration with Notion  
- Real-world AI agent workflow implementation  

---

