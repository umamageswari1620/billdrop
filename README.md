# BillDrop
Supplier bills into clean, checked records in minutes.

## Live link
https://umamageswari1620.github.io/billdrop/

## Test logins (made-up, demo only)
- Accountant: accountant@example.com
- Manager: manager@example.com
- Passwords: shared privately, not in this file

## What works
- Login for accountant and manager, with role shown after login
- Single bill: upload, OCR read, AI fields, review, save
- Batch upload of up to 20 bills, with a card for each bill
- Wrong total check (bill-05: "Total is off by ₹1800")
- Duplicate check against the database
- Save All Clean Bills, and save each card one by one
- Download Excel and supplier totals for this month

## Partly works
- AI reading sometimes fails (503, 429), so fields come from OCR and need checking
- Supplier names: OCR spelling differences can create separate suppliers

## Not built yet
- 10 automated tests in GitHub Actions
- AI draft message for wrong-total bills
- Background processing (batch stops if the tab is closed)

## M4 deliverables
- **Live link:** https://umamageswari1620.github.io/billdrop/
- **2-minute video:** https://drive.google.com/file/d/1lGqjh9LIgOu2TuhxfFfHK0I66yadtUYn/view
- **20-bill batch recording:** https://drive.google.com/file/d/1VkFDCk8L6rmhY_YTln4bCp1l8TZePHjs/view
- **docs/AI_NOTES.pdf:** https://github.com/umamageswari1620/billdrop/blob/main/docs/AI_NOTES (1).pdf
- **docs/SPEED.png:** https://github.com/umamageswari1620/billdrop/blob/main/docs/SPEED.png
- **docs/PROGRESS.pdf:** https://github.com/umamageswari1620/billdrop/blob/main/docs/PROGRESS.pdf
- **docs/REAL_USERS.pdf:** https://github.com/umamageswari1620/billdrop/blob/main/docs/REAL_USERS.pdf
- **docs/PLAN.pdf:** https://github.com/umamageswari1620/billdrop/blob/main/docs/PLAN.pdf
## Tech used
HTML and JavaScript, Supabase (database, login, row level security), Tesseract.js (OCR), Gemini AI through a Supabase Edge Function.
