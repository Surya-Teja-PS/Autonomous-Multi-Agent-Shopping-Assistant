# Autonomous-Multi-Agent-Shopping-Assistant
This is the brief one-liner that sits right below your repository name on the main page. It needs to be punchy and keyword-rich.  An autonomous, multi-agent AI shopping assistant orchestrated via n8n, Gemini 3.5-flash, and ScraperAPI for high-throughput query automation.

🛒 Autonomous Multi-Agent Shopping Assistant
A resilient, multi-agent AI pipeline engineered to autonomously orchestrate, route, and resolve complex retail queries with sub-second latency.

📖 Executive Summary
The Autonomous Multi-Agent Shopping Assistant is a high-throughput conversational AI system designed to streamline retail research and data extraction. Moving beyond simple wrapper applications, this project introduces a robust, multi-branch workflow architecture that intelligently distributes tasks between specialized LLM agents and web scrapers.

By migrating core inference nodes to Gemini 3.5-flash and Groq, and implementing custom fault-tolerance mechanisms, the system achieves massive latency reductions while maintaining near-perfect uptime during automated data retrieval.

⚡ Engineering Impact & Performance Metrics
High-Throughput Orchestration: Engineered a scalable agentic system via Groq & ScraperAPI automating 200+ daily queries, cutting latency 95%.

Fault-Tolerant Design: Eliminated critical system failures by engineering 2-level automated retry logic & error monitoring workflows.

Dynamic Task Routing: Developed a conversational AI assistant using 4+ logic branches in n8n to dispatch 100+ user requests each week.

Cost & Speed Optimization: Optimized daily AI throughput by migrating 5+ complex workflow nodes to high-efficiency Gemini 3.5-flash.

🏗️ System Architecture
(Pro-Tip for your GitHub: Export a screenshot of your n8n workflow canvas and replace [architecture-diagram.png] with the actual image path. Visualizing the workflow is highly impressive to recruiters).

Core Components
Ingestion Layer: Captures dynamic user requests and standardizes the payload for downstream processing.

Logic & Routing Engine (n8n): Evaluates intent and triggers 1 of 4 specialized workflow branches based on query complexity.

Inference Layer:

Groq: Handles rapid natural language understanding and initial entity extraction.

Gemini 3.5-flash: Executes complex reasoning, synthesizes scraped data, and generates the final conversational response.

Data Extraction Layer (ScraperAPI): Bypasses IP blocks and captchas to autonomously gather real-time pricing and product data.

🛡️ Reliability & Error Handling
Standard LLM pipelines frequently fail due to API rate limits or malformed scraper responses. This architecture solves that through a custom 2-Level Retry Logic Workflow:

Level 1 (Soft Retry): Intercepts API timeouts and initiates an immediate exponential backoff retry.

Level 2 (Fallback Execution): If the primary data node fails, the workflow redirects to a fallback search agent, logs the error payload to a monitoring channel, and successfully completes the user request without a system crash.

🚀 Quick Start & Deployment
Prerequisites
n8n instance (Local or Cloud)

API Keys for Google AI Studio (Gemini), Groq, and ScraperAPI

![System Architecture](Screenshot%202026-07-14%20230757.png)


