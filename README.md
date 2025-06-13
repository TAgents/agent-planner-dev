# Agent Planner Development Environment Setup

This guide will help you set up the local development environment for the agent-planner software.

## Prerequisites

- Docker and Docker Compose
- The following project directories should exist parallel to this one:
  - `agent-planner`
  - `agent-planner-agents`
  - `agent-planner-mcp`
  - `agent-planner-ui`

## Setup Instructions

### 1. Environment Variables

Copy the example environment file and configure it:

```bash
cp .env--example .env
```

Edit the `.env` file and update the following:
- `GOOGLE_API_KEY`: Get from https://ai.google.dev/
- `PLANNING_API_TOKEN`: Generate after system is running
- `USER_API_TOKEN`: Generate after system is running

### 2. SSL Certificates

The development environment uses HTTPS with local certificates. Ensure certificates exist in the `local-certs/` directory:
- `cert.pem`
- `key.pem`
- `dynamic.yml`
