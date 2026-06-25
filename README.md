Auto SOP Ticketing System

An automated ticketing and Standard Operating Procedure (SOP) platform that streamlines incident response by generating tickets, assigning priorities, and providing step-by-step remediation guidance.

Overview

The Auto SOP Ticketing System is designed to improve IT and cybersecurity operations by reducing manual work during incident handling. Instead of requiring analysts to search through documentation, the system automatically creates tickets, categorizes issues, determines severity, and attaches the appropriate Standard Operating Procedure (SOP).

This project demonstrates practical skills in:

Python development
REST API integration
Automation
IT Service Management (ITSM)
Cybersecurity workflows
Documentation
Logging and auditing

This repository is intended as a portfolio project for employers interested in Network Security, SOC, Help Desk, or Systems Administration candidates.

Features
Automatic ticket creation
Incident categorization
Severity and priority assignment
SOP recommendation engine
Ticket status tracking
User authentication
Audit logging
Dashboard for ticket management
Email notifications (optional)
REST API support
JSON-based ticket storage (upgradeable to SQL)
Example Workflow
Alert Received
       │
       ▼
Auto Ticket Generated
       │
       ▼
Incident Categorized
       │
       ▼
Priority Assigned
       │
       ▼
Correct SOP Attached
       │
       ▼
Assigned to Technician
       │
       ▼
Resolution Logged
       │
       ▼
Ticket Closed
Tech Stack
Component	Technology
Backend	Python
API	Flask / FastAPI
Database	SQLite or PostgreSQL
Frontend	HTML, CSS, JavaScript
Authentication	JWT
Logging	Python Logging
Version Control	Git
Documentation	Markdown
Project Structure
Auto-SOP-Ticketing-System/
│
├── app/
│   ├── routes/
│   ├── models/
│   ├── services/
│   ├── auth/
│   ├── templates/
│   ├── static/
│   └── database.py
│
├── sop_library/
│   ├── Password_Reset.md
│   ├── Malware_Response.md
│   ├── VPN_Issue.md
│   ├── Account_Lockout.md
│   └── Network_Outage.md
│
├── tickets/
│
├── logs/
│
├── tests/
│
├── config.py
├── requirements.txt
├── run.py
└── README.md
Ticket Fields

Each ticket contains:

{
    "ticket_id": "INC-1001",
    "title": "VPN Connection Failure",
    "category": "Network",
    "priority": "High",
    "status": "Open",
    "assigned_to": "Network Team",
    "created_at": "2026-06-25",
    "recommended_sop": "VPN_Issue.md"
}
Severity Levels
Severity	Description
Critical	Organization-wide outage or security incident
High	Major service disruption
Medium	Single-user issue affecting productivity
Low	Minor request or informational ticket
Sample SOP Library
SOP	Description
Password Reset	Active Directory password reset procedure
Malware Response	Endpoint isolation and malware removal
VPN Troubleshooting	VPN connectivity issues
Account Lockout	Unlocking user accounts
Network Outage	Diagnosing network connectivity failures
API Endpoints
Create Ticket
POST /api/tickets
Request
{
    "title": "VPN Failure",
    "category": "Network"
}
Response
{
    "ticket_id": "INC-1001",
    "priority": "High",
    "recommended_sop": "VPN_Issue.md"
}
Get Ticket
GET /api/tickets/{id}
Update Ticket
PUT /api/tickets/{id}
Close Ticket
DELETE /api/tickets/{id}
Installation

Clone the repository

git clone https://github.com/yourusername/Auto-SOP-Ticketing-System.git

Navigate into the project

cd Auto-SOP-Ticketing-System

Install dependencies

pip install -r requirements.txt

Run the application

python run.py
Future Improvements
Active Directory integration
Microsoft Entra ID integration
ServiceNow integration
Jira integration
AI-powered ticket classification
AI-generated remediation suggestions
Email automation
Microsoft Teams notifications
Slack notifications
Docker deployment
Kubernetes deployment
RBAC (Role-Based Access Control)
Multi-tenant support
SIEM integration (Splunk, Microsoft Sentinel, QRadar)
Syslog ingestion
LDAP authentication
Screenshots
Coming Soon
Learning Objectives

This project demonstrates knowledge of:

ITIL incident management
Standard Operating Procedures
Network troubleshooting
REST API development
Authentication
Secure coding practices
Logging and monitoring
Backend architecture
Software documentation
Version control with Git
Potential Use Cases
IT Help Desk
SOC Analyst workflows
Managed Service Providers (MSPs)
Internal IT departments
Network Operations Centers (NOCs)
Cybersecurity incident response
Educational labs
Home lab automation
License

This project is licensed under the MIT License.


Eric Rutherford

Cybersecurity Devoloper | Network Security Engineer

Why This Project Matters

Modern IT teams often waste valuable time manually creating tickets and searching for documentation. This project automates that process by pairing incident management with standardized response procedures, helping technicians resolve issues faster while maintaining consistency and compliance. It serves as both a practical operations tool and a portfolio project showcasing backend development, automation, and cybersecurity fundamentals.
