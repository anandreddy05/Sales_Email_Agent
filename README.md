# Cold Email Automation with Multi-Agent GPT-4o Workflow

Automatically generate, compare, and send cold sales emails using multiple AI agents and SendGrid integration. This project showcases an intelligent multi-agent system that drafts cold outreach emails, ranks them, and sends only the best one—fully autonomously.

## What This Project Does

This system simulates a smart AI sales team:

Three GPT-4o agents (professional, humorous, concise) independently write cold sales emails.

A fourth agent ("email picker") reviews and selects the most effective version.

The winning email is automatically sent via the SendGrid email API.

Use case: Cold outreach for ComplAI, an AI-powered SaaS product that helps businesses with SOC2 compliance.

## Agents in Action

Agent	Style	Role

- Professional Sales Agent	Formal & serious	Writes polished, audit-focused emails
- Engaging Sales Agent	Witty & informal	Crafts funny and attention-grabbing emails
- Busy Sales Agent	Direct & concise	Writes fast, no-nonsense emails
- Email Picker Agent	Judgmental customer persona	Picks the email most likely to get a reply

All agents are powered by OpenAI’s GPT-4o-mini model for speed and cost efficiency.

##  Tech Stack

- OpenAI GPT-4o-mini: Core LLM engine
- SendGrid API: Sends selected cold email to a target inbox
- Custom Agent, Runner, and function_tool abstractions (assumed internal modules)
- asyncio: Run agent calls in parallel
- .env config: API key and email credentials

