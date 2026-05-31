# -n8n-Workflow
# Earthonoid AI – Intern Assignment
**By:** Vishh | codewithvishh@gmail.com

---

## What I Built
A lead capture automation using n8n that:
- Takes data from a web form
- Saves it to Google Sheets
- Sends a confirmation email automatically
- Handles errors if name or email is missing

---

## How It Works
## How to Run It
1. Install Docker
2. Run n8n:
   docker run -p 5678:5678 n8nio/n8n
3. Open http://localhost:5678
4. Import My_workflow.json
5. Connect Google Sheets + Gmail
6. Hit Activate — done!

## Quick Test
```powershell
Invoke-RestMethod -Uri "http://localhost:5678/webhook-test/lead-capture" -Method POST -ContentType "application/json" -Body '{"name":"Vishh","email":"codewithvishh@gmail.com","phone":"9876543210","message":"Hello!"}'
```

## What You'll See
- New row in Google Sheets ✅
- Confirmation email in inbox ✅
- JSON success response ✅

## Tools Used
n8n · Google Sheets · Gmail · Docker
