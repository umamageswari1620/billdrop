## M3 status (honest)

**Working**
- Batch upload of up to 20 bills, with a card for each bill
- OCR read and AI fields, with fallback reader when AI is busy
- Wrong total check (bill-05: "Total is off by ₹1800")
- Duplicate check against the database
- Save All Clean Bills, and save each card one by one
- Download Excel (billdrop-batch.xlsx)
- Supplier totals for this month

**Partly working**
- AI reading sometimes fails (503, 429), so fields come from OCR and need checking
- Supplier names: OCR spelling differences can create separate suppliers

**Not built yet**
- 10 automated tests in GitHub Actions
- AI draft message for wrong-total bills
- Background processing (batch stops if the tab is closed)

**Testers**
- 10 people tried the tool. Feedback in `docs/REAL_USERS.pdf`.
