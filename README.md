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

# Introduction
Learning a new skill often involves searching through multiple resources, identifying relevant topics, and structuring them into a proper roadmap. This process can be time-consuming and unstructured.

This project was developed to solve this problem by automating the creation of personalized learning paths. By leveraging AI agents and workflow automation, the system takes a skill as input, researches relevant resources, and generates a structured plan with actionable steps.

The output is directly stored in Notion as a task tracker, making it practical and easy to follow.

---

## Objective
The goal of this project is to:
- Automate the process of researching and structuring learning resources
- Eliminate manual effort in searching and organizing study plans
- Build a practical AI agent capable of **tool usage and workflow automation**

---

# Introduction
Learning a new skill often involves searching through multiple resources, identifying relevant topics, and structuring them into a proper roadmap. This process can be time-consuming and unstructured.

This project was developed to solve this problem by automating the creation of personalized learning paths. By leveraging AI agents and workflow automation, the system takes a skill as input, researches relevant resources, and generates a structured plan with actionable steps.

The output is directly stored in Notion as a task tracker, making it practical and easy to follow.

---

## Workflow Architecture
The workflow follows this pipeline:
Chat Trigger → AI Agent → (Search Tool + Notion Tool)

### 1. User Input
The workflow begins when the user provides a **skill to learn** through the chat trigger node.
Example input: Machine Learning

### 2. Main AI Agent
The **Main AI Agent** acts as the controller of the workflow. It processes the user input and determines how to generate the learning path.
It uses a chat model to reason, plan, and decide when to call tools.

### 3. Chat Model
The AI agent is powered by a chat model that enables it to:
- Understand user intent  
- Generate structured learning steps  
- Decide tool usage  

### 4. Web Search Tool (SerpAPI)
The AI agent uses the **SerpAPI** tool to perform web searches and gather relevant learning resources.
This ensures that the generated learning path is based on up-to-date and high-quality content.

### 5. Learning Path Generation
After collecting relevant information, the AI agent generates a structured learning path consisting of:
- Sub-topic based tasks (not generic steps)  
- Clear descriptions for each task  
- Priority levels  
- Effort estimation  

### 6. Notion Integration
The generated learning tasks are automatically stored in a Notion task tracker database.
Each task includes:
- Task Name (sub-topic)  
- Description  
- Status (Pending)  
- Priority  
- Effort Level  
- Assignee (me)  
- Due Date  

---

# Technologies Used

- **n8n** – Workflow automation platform  
- **OpenRouter** – AI chat model integration  
- **SerpAPI** – Web search API  
- **Notion API** – Task management and storage  

---

# AI Agent Design

This project uses a structured AI agent design to ensure efficient workflow execution.

### Main AI Agent
- Interprets user input  
- Controls workflow execution  
- Generates structured learning tasks  

### Tool Integration
- Uses search tool to gather learning resources  
- Uses Notion tool to store structured outputs  

This design ensures modularity, scalability, and better control over AI behavior.

---

# Project Demonstration

A complete demonstration of the workflow is available in the video below:

**Video Demonstration:**  
https://drive.google.com/

The demonstration includes:

- Explanation of the project  
- Overview of workflow nodes  
- Live execution of the workflow  
- AI agent tool usage  
- Notion task creation  

---

# Workflow File

**Workflow JSON File**

The repository contains the exported workflow JSON file.

Steps to use:
1. Open your n8n workspace  
2. Import the JSON file  
3. Configure API credentials (SerpAPI, Notion, etc.)  
4. Run the workflow  

This allows easy replication of the project.

---

# Challenges Faced

### AI Agent Not Using Tools
Initially, the AI agent generated responses without calling tools. This was resolved by refining system prompts and tool descriptions.

### Schema Mismatch Errors
The Notion node produced errors due to mismatched input formats. This was solved by simplifying the AI output and handling structured fields within n8n.

### API Integration Issues
Authentication errors occurred with external APIs. Proper credential configuration resolved these issues.

### Handling Multiple Fields
Passing too many fields through the AI caused failures. The solution was to limit AI output and map fields within the workflow.

---

# Future Improvements

- Integration with YouTube API for better video recommendations  
- Dynamic due date assignment  
- Multi-skill learning path generation  
- Integration with additional task management tools  
- Development of a user interface  

---

# Conclusion

This project demonstrates how AI agents can be combined with workflow automation to create intelligent and practical systems.

By automating the process of researching and structuring learning paths, this system significantly reduces manual effort and improves productivity.

The project highlights the real-world potential of AI-driven automation in education and skill development.
