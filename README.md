# DevOps Agent

AI-powered DevOps agent that collects operational data and sends intelligent notifications.

## Data Sources (Collectors)
- **CloudWatch** — AWS metrics & alarms
- **Datadog** — APM, infrastructure monitoring
- **Splunk** — Log analysis
- **Confluence** — Runbooks & knowledge base (RAG)

## Notification Targets
- **Slack** — Team alerts
- **PagerDuty** — On-call escalation
- **Microsoft Teams** — Channel notifications

## Project Structure
```
devops-agent/
├── src/
│   ├── agents/       # AI agent orchestration
│   ├── collectors/   # Data source integrations
│   ├── notifiers/    # Notification integrations
│   └── rag/          # RAG (Confluence knowledge retrieval)
├── config/           # Configuration files
├── infra/            # IaC (CDK / Terraform)
├── tests/
└── docs/
```

## Setup
```bash
cp .env.example .env
# Fill in credentials in .env

pip install -r requirements.txt
python src/agents/main.py
```
