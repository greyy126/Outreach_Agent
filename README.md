# Outreach Agent | AI Powered Cold Outreach System

AI agent that converts job listings into highly personalized referral outreach emails by combining job parsing, company context extraction, contact discovery, and LLM driven writing with human in the loop control.

---

## Problem

Cold outreach is slow, manual, and inconsistent.

Most candidates:
- spend hours researching roles  
- struggle to find the right contact  
- send generic emails that get ignored  

---

## Solution

This agent automates the entire outreach workflow from job discovery to email draft creation while keeping human judgment in key steps.

It is designed to optimize for one outcome:  
**getting replies, not just sending emails**

---

## Workflow
<img width="678" height="734" alt="Email_drafter_agent_workflow" src="https://github.com/user-attachments/assets/aeef4724-4c70-4b34-a414-8398bbd31238" />


---

## Key Features

- **Job aware personalization**  
  Extracts role requirements and aligns messaging to the job  

- **Company specific hooks**  
  Uses real signals like product, initiative, or positioning  

- **Contact intelligence**  
  Identifies relevant hiring managers or recruiters  

- **Email enrichment**  
  Uses Hunter MCP with confidence thresholds and fallback logic  

- **Human in the loop control**  
  Requires approval before processing and before sending  

- **Single angle storytelling**  
  Ensures focused, high quality narrative instead of generic bullets  

---

## Tech Stack

- LLM: Claude  
- Data Source: Jobright (GitHub job listings)  
- Contact Enrichment: Hunter MCP  
- Output: Gmail Drafts / LinkedIn Messages  

---

## Example Output

**Subject:** Data Analyst Role at Company  

Hi [First Name],  
I came across the Data Analyst role at [Company] and wanted to reach out directly — noticed how your team is focusing on [specific product/initiative].

I’m Gresha, a recent Information Science graduate from UW Madison. A few things I’ve worked on that might be relevant:

- Built an automated data pipeline reducing manual effort by 70% while improving data reliability across sources  
- Developed dashboards using Power BI to track performance metrics across multiple datasets  
- Ran marketing analytics experiments that improved campaign conversion by 10%  

I'd love to connect if there's a moment to chat. I've attached my resume for reference.  

---

## Design Principles

- Minimal input → maximum personalization  
- One strong narrative > multiple weak points  
- Specific context > generic messaging  
- Automation + human judgment > blind automation  

---

## Failure Handling

The agent stops execution if:
- Job description cannot be fetched  
- No valid contact is found  
- Email confidence is too low  
- Required inputs are missing  

---

## Why this matters

Most outreach tools optimize for volume.  
This system optimizes for quality and response rate by combining structured workflows with LLM reasoning and controlled execution.

