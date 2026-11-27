# Pawcare – Community Pet Appointment Tracker

A one-page appointment tracker for a community veterinary clinic. Staff can add, view, edit, complete, cancel, and delete appointments. It stores appointments in the current browser with `localStorage`; it needs no account, server, database, or installation.

## Community problem

**Working assumption to confirm with a clinic staff member:** In our local veterinary clinic, staff can struggle to keep track of upcoming pet visits when details are written in separate notes. A single appointment list could help staff record and check scheduled visits.

Do not present this as an interviewed or verified community need unless you have checked it with someone who has the problem. The demo uses made-up names only.

## Target users

The primary users are staff at a small community veterinary clinic who schedule and track visits. Pet owners are represented only by fictional names in the class demo; this app is not for real client records.

## FR-01

**FR-01:** Clinic staff can add, view, edit, update the status of, and delete an appointment with the pet name, owner name, appointment date, time, and reason for visit. Each appointment has a Pending, Completed, or Cancelled status.

### Acceptance criteria

1. A valid appointment is added to the list and saved in this browser with Pending status.
2. Pet name, owner name, date, time, and reason are required; blank and whitespace-only names/reasons are rejected with a clear message.
3. An invalid calendar date or a date before today is rejected with a clear message.
4. Staff can change status to Pending, Completed, or Cancelled; the choice is saved.
5. Staff can edit appointment details or delete an appointment; each change is saved.
6. After refreshing the page in the same browser, saved appointments and their status remain visible.

## Features

- Add and view appointments in date-and-time order.
- Edit appointment details and cancel an unsaved edit.
- Change status to Pending, Completed, or Cancelled.
- Delete an appointment after confirming the action.
- Reject blank or whitespace-only required fields and past dates with a message.

## Scope and use

This app implements one feature: managing pet appointments. Enter made-up demo data, select today or a future date, and choose **Add appointment**. Use each appointment card's status menu, **Edit**, or **Delete** controls. Editing keeps the existing status; deleting asks for confirmation. The list is ordered by date and time. There are no owner accounts, medical records, payments, or synchronization between devices.

## Run it

Open `index.html` in a modern browser. No packages or build step are needed. If opening a local file does not allow browser storage in your browser, serve the folder locally, for example:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Technologies

- HTML provides the form and appointment list.
- CSS provides the green-and-white responsive layout.
- Plain JavaScript handles validation, rendering, editing, status changes, and deletion.
- Browser `localStorage` stores appointment data as JSON.

## localStorage architecture

When `index.html` opens, JavaScript reads the `pawcare-appointments-v1` key from the current browser's `localStorage` and renders the saved appointments. Adding, editing, changing status, or deleting writes the updated list back to that key. The data stays in that browser profile; it is not uploaded or backed up, and clearing site data can remove it. If stored data cannot be read, the page reports the problem and disables saving rather than overwriting the data. There is no server, login, database, framework, or external API.

## Manual test table

Use made-up values only. Clear the app's localStorage between independent runs if needed.

| # | Test | Expected result | Result |
|---|---|---|---|
| 1 | Submit a valid appointment with all required fields | Appointment appears with Pending status and a success message | Pass |
| 2 | Leave each required field blank in turn (pet, owner, date, time, reason) | No appointment is added and a helpful error appears | Pass |
| 3 | Enter only spaces for the pet name, owner name, or reason | No appointment is added and a helpful error appears | Pass |
| 4 | Choose a date before today | No appointment is added and the date rule is explained | Pass |
| 5 | Try an invalid calendar date, such as February 30 | The app rejects it | Pass |
| 6 | Change status to Completed, Cancelled, and Pending | Each selection updates the saved appointment | Pass |
| 7 | Edit the name and reason, then save | Updated details appear; current status is kept | Pass |
| 8 | Edit a field, then cancel editing | Original appointment remains unchanged | Pass |
| 9 | Refresh after editing and changing status | Updated details and status remain visible | Pass |
| 10 | Delete an appointment and confirm when another appointment remains | The selected appointment is removed and the remaining appointment stays visible | Pass |
| 11 | Load malformed localStorage data | Page stays usable, explains the issue, and disables saving to prevent overwrite | Pass |
| 12 | Enter markup-like text as a pet name | It appears as text and does not create page markup | Pass |
| 13 | View the page at widths from 320px to desktop, with long fictional names | No horizontal scrolling or overlap; forms and appointment controls stay readable | Pass |
| 14 | Delete the last appointment and check the empty state | The appointment is removed and the empty-state message appears | Not yet tested |

Test 5 exercised the date check after changing the input control to text in the browser test; normal date controls also prevent selecting nonexistent calendar dates.

## Submission links

- Public repository: https://github.com/huralrheamae-jpg/Animals-Clinic
- YouTube demo: add your public 2–3 minute video link after recording it with made-up data.
