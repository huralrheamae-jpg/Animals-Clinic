# Pawcare – Community Pet Appointment Tracker

## Pitch

Pawcare gives a small community veterinary clinic one simple page to organize pet appointments without a server or account.

## Problem

**Working assumption to confirm:** In our local veterinary clinic, appointment details may be scattered across notes, making upcoming visits harder to check in one place. A single browser-based appointment list could make scheduling easier. This is a project assumption, not a claim that a community member has already been interviewed.

## Target users

The primary users are clinic staff who schedule and track visits. Pet owners are represented only by fictional names; the class demo is not intended for real client or medical data.

## Main feature · FR-01

Clinic staff can add, view, edit, change the status of, and delete an appointment. Each appointment contains a pet name, owner name, date, time, reason, and Pending, Completed, or Cancelled status.

**FR-01:** Clinic staff can manage a pet appointment with the pet name, owner name, appointment date, time, reason for visit, and status.

## Technologies and architecture

One `index.html` file contains the HTML, responsive CSS, and plain JavaScript. JavaScript validates the form and renders and updates the appointment list. It reads and writes JSON in the browser's `localStorage` key `pawcare-appointments-v1`. Data remains in that browser profile; it is not sent to a server and may be lost if site data is cleared. The project uses no framework, backend, database, or external API.
