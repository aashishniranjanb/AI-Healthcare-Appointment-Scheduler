# Environment Setup for Wellspring Clinic AI Scheduler

## Overview
This document describes the necessary environment variables and configuration parameters required to deploy the Healthcare AI Appointment Scheduler.

---

## Required Environment Variables

| Variable Name                 | Description                                              | Example Value                          |
|------------------------------|----------------------------------------------------------|--------------------------------------|
| VAPI_API_KEY                 | API key for accessing Vapi AI assistant services         | `sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`  |
| GOOGLE_CALENDAR_API_URL      | Base URL for Google Calendar API endpoints                | `https://www.googleapis.com/calendar/v3` |
| GOOGLE_SERVICE_ACCOUNT_JSON  | Path or content of Google service account credentials     | `./credentials/service-account.json` |
| MAKE_COM_CHECK_AVAIL_WEBHOOK | Webhook URL for availability checking Make.com scenario  | `https://hook.make.com/xyz123`       |
| MAKE_COM_BOOK_APPT_WEBHOOK   | Webhook URL for booking appointment Make.com scenario     | `https://hook.make.com/abc456`       |
| DEEPGRAM_API_KEY             | API key for Deepgram transcription service                | `dg_XXXXXXXXXXXXXXXXXXXXXXXX`        |
| ELEVENLABS_API_KEY           | API key for ElevenLabs voice synthesis                     | `elevenlabs_XXXXXXXXXXXXXXXXXXXX`   |

---

## Setup Instructions

1. Ensure all API keys are kept secure and are not exposed in public repositories.
2. Store the Google service account JSON securely; use encrypted secrets or managed vault solutions where possible.
3. Load environment variables into your deployment environment before starting any services.
4. Verify API key permissions, especially scopes for calendar and voice services.
5. Regularly rotate keys per security best practices.

---

## Optional Variables

| Variable Name             | Description                                          | Example Value          |
|--------------------------|------------------------------------------------------|------------------------|
| LOG_LEVEL                | Defines logging verbosity (e.g., DEBUG, INFO, ERROR) | `INFO`                 |
| MAX_CALL_DURATION        | Maximum call length in seconds                       | `600`                  |

---

# End of Environment Setup
