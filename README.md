# Pawcare Appointment Book

A one-page appointment tracker for a community veterinary clinic. It stores appointments in the current browser with `localStorage`; it needs no account, server, database, or installation.

## Community problem

**Working assumption to confirm with a clinic staff member:** In our local veterinary clinic, staff can struggle to keep track of upcoming pet visits when details are written in separate notes. A single appointment list could help staff record and check scheduled visits.

Do not present this as an interviewed or verified community need unless you have checked it with someone who has the problem. The demo uses made-up names only.

## FR-01

**FR-01:** Clinic staff can schedule and view an appointment containing the pet name, owner name, appointment date, time, and reason for visit.

### Acceptance criteria

1. A valid appointment is added to the list and saved in this browser.
2. Pet name, owner name, date, time, and reason are required; blank and whitespace-only names/reasons are rejected.
3. An invalid calendar date or a date before today is rejected.
4. After refreshing the page in the same browser, saved appointments remain visible.

## Scope and use

This app implements one feature: scheduling and viewing pet appointments. Enter made-up demo data, select today or a future date, and choose **Add appointment**. The list is ordered by date and time. There are no owner accounts, medical records, payments, appointment editing, or synchronization between devices.

## Run it

Open `index.html` in a modern browser. No packages or build step are needed. If opening a local file does not allow browser storage in your browser, serve the folder locally, for example:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Architecture

- `index.html` contains the page structure, responsive CSS, form validation, appointment rendering, and storage logic.
- Vanilla JavaScript validates appointment fields and writes JSON to the browser's `localStorage`.
- Data stays in that browser profile; it is not uploaded or backed up. Clearing site data can remove it.
- The app has no external dependencies, server, login, or database.

## Manual test table

Use made-up values only. Clear the app's localStorage between independent runs if needed.

| # | Test | Expected result | Result |
|---|---|---|---|
| 1 | Submit a valid appointment with all five fields | One appointment appears in the list and the count updates | Pass |
| 2 | Leave a required field blank and submit | Browser validation prevents the save | Pass |
| 3 | Enter only spaces for a required name or reason | The app rejects the value and shows an error | Pass |
| 4 | Choose a date before today | The app rejects the appointment and explains the date rule | Pass |
| 5 | Use an invalid calendar date, such as February 30 | The app rejects the date | Pass |
| 6 | Refresh after saving a valid appointment | The appointment remains visible in the same browser | Pass |
| 7 | Enter markup-like text as a name | It appears as text and does not create page markup | Pass |

Test 5 exercised the date check after changing the input control to text in the browser test; normal date controls also prevent selecting nonexistent calendar dates.

## Submission links

- Public repository: https://github.com/huralrheamae-jpg/Animals-Clinic
- YouTube demo: add your public 2–3 minute video link after recording it with made-up data.
