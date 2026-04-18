# Iris Backend

FastAPI backend for Iris — AI email & calendar assistant.

## Features
- Gmail IMAP scanning
- Appointment detection (French & English)
- Microsoft Graph API (Outlook) support
- Calendar integration

## Setup
```bash
pip install -r requirements.txt
python main.py
```

## Environment Variables
- `GMAIL_ADDRESS` — your Gmail address
- `GMAIL_APP_PASSWORD` — Gmail app password (16 chars)
- `AZURE_CLIENT_ID` — for Outlook support
- `AZURE_CLIENT_SECRET` — for Outlook support
- `AZURE_TENANT_ID` — for Outlook support

## API Endpoints
- `POST /api/gmail/scan` — scan Gmail inbox
- `POST /api/gmail/appointments` — get detected appointments
- `GET /api/gmail/setup-guide` — setup instructions
