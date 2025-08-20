# Wellspring Clinic Google Calendar Setup Instructions

## Overview
This document guides you through setting up the Google Calendar required for the Wellspring Clinic AI Appointment Scheduler.

---

## Step 1: Create a New Calendar
1. Go to [Google Calendar](https://calendar.google.com).
2. On the left sidebar, click the **"+"** button next to "Other calendars".
3. Select **Create new calendar**.
4. Name the calendar: **Wellspring Clinic**.
5. Add description (optional): "Appointment scheduling calendar for Wellspring Clinic AI Assistant".
6. Select appropriate Time zone.
7. Click **Create calendar**.

---

## Step 2: Configure Business Hours
1. In Google Calendar, click the **Settings (gear icon)**.
2. Select **Working hours & location**.
3. Turn on **Enable working hours**.
4. Specify:
   - Monday to Friday
   - From 8:00 AM to 6:00 PM
5. Save your settings.

---

## Step 3: Access and Share Settings
1. Go to the Wellspring Clinic calendar settings.
2. Under **Access permissions**, enable access as required for your team.
3. For integrations like Make.com or backend services, create a service account or use OAuth authentication with proper API consent.

---

## Step 4: API Access Setup
1. Visit the [Google Cloud Console](https://console.cloud.google.com/).
2. Create or select an existing project.
3. Enable the **Google Calendar API**.
4. Under **Credentials**, create an **OAuth 2.0 Client ID** or a **Service Account**, depending on your app.
5. Download the credentials JSON file.  
   This file will be used for authenticated API access from Make.com or your backend.

---

## Step 5: Testing Your Setup
- Test by creating a manual event.
- Use Google Calendar API test tools or integrate with Make.com workflow to check calendar access.
- Verify that API calls can create, read, and update events in the Wellspring Clinic calendar.

---

**Note:**  
For secure and reliable access, make sure API credentials are stored securely and only authorized personnel have access.

---

# End of Setup Instructions
