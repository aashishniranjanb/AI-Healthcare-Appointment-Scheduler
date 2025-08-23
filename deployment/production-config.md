# Production Deployment Guide for Wellspring Clinic AI Scheduler

## System Architecture

- AI Voice Assistant runs on Vapi.ai managed service
- Automation workflows executed by Make.com
- Google Calendar API integration for appointment event management
- Backend server (optional) for additional business logic or data storage
- Web widget hosted on the client’s website or platform

---

## Deployment Steps

### 1. Prepare Environment

- Configure all environment variables as per `environment-setup.md`
- Ensure API keys and credentials have correct scopes and permissions

### 2. Backend Services (if any)

- Deploy backend server (Node.js, Python, or other) on a secure environment such as AWS, Azure, or GCP
- Use HTTPS with TLS certificates for all server communication
- Implement authentication and audit logging

### 3. Vapi.ai Assistant Setup

- Import the assistant configuration JSON
- Update Server URLs of custom tools with production webhook endpoints
- Enable HIPAA mode and privacy features
- Set call timeout policies

### 4. Make.com Scenario Deployment

- Import automation scenarios for availability check and booking
- Update Google Calendar connections with production credentials
- Test webhook URLs for production readiness

### 5. Web Widget Integration

- Deploy widget JavaScript snippet on the production website
- Customize colors and button text to match corporate branding

### 6. Testing & Validation

- Perform end-to-end testing in production environment
- Validate response times, booking accuracy, and error handling
- Verify data privacy compliance and audit logs

---

## Monitoring & Maintenance

- Monitor API usage and error logs on Vapi and Make.com dashboards
- Set up alerting for failures or anomalies
- Schedule regular audits for HIPAA compliance
- Keep dependency versions and credentials up to date

---

## Rollback Plan

- Maintain backups of previous assistant and workflow versions
- Use feature flags to disable new features if issues arise
- Coordinate communication with stakeholders for downtime events

---

# End of Production Deployment Guide
