# Pawcare Appointment Book · Project brief

## Pitch

One simple page helps community veterinary clinic staff keep upcoming pet visits together without a server or account.

## Problem

**Working assumption to confirm:** In our local veterinary clinic, appointment details may be scattered across notes, making upcoming visits harder to check in one place. A single browser-based appointment list could make scheduling easier. This is a project assumption, not a claim that a community member has already been interviewed.

## Users

Primary user: veterinary clinic staff who schedule visits. The demo uses made-up pet and owner names only; it is not intended for real client or medical data.

## Feature and requirement

The app implements one feature: schedule and view a pet appointment.

**FR-01:** Clinic staff can schedule and view an appointment containing the pet name, owner name, appointment date, time, and reason for visit.

## Architecture

One `index.html` file contains the HTML form, responsive CSS, and vanilla JavaScript. JavaScript validates fields, renders the appointment list, and stores appointment JSON in the browser's `localStorage`. Nothing is sent to a server. Data is limited to the browser profile and may be lost if its site data is cleared.
