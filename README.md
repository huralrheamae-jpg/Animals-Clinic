# Pawcare Clinic

Pawcare Clinic is a lightweight, browser-based animal clinic management system. It brings pet and owner information, appointments, and medical history together in one responsive interface.

## Purpose

The application helps a clinic keep track of registered pets and their owners, schedule and update appointments, and record diagnoses, treatments, and vaccinations. A dashboard gives a quick overview of clinic activity.

## Features

- **Dashboard:** View total pets, owners, appointments, and completed checkups, plus recent pets and upcoming appointments.
- **Pet registration:** Record a pet's name, type, breed, age, sex, and owner.
- **Owner management:** Store owner names, phone numbers, email addresses, and addresses.
- **Appointments:** Schedule appointments for registered pets, record the visit date, time, and reason, and update appointment status.
- **Medical records:** Keep dated diagnosis, treatment, and vaccination information for each pet.
- **Pet search:** Find registered pets by name.
- **Record deletion:** Remove owners, pets, appointments, or medical records. Deleting a pet also deletes its linked appointments and medical records.
- **Browser storage:** Save records in the browser's `localStorage` so they remain available after a refresh in the same browser.
- **Responsive layout:** Use the interface on desktop and mobile screen sizes.

## Requirements

- A modern web browser with JavaScript and browser storage enabled.
- No package manager, dependencies, database server, or build tools are required.

## Installation and setup

1. Download or clone this project.
2. Keep `index.html` in the project directory.
3. Open the file in a modern browser, or serve the project directory locally. For example, if Python is installed:

   ```bash
   python -m http.server 8000
   ```

4. Visit [http://localhost:8000](http://localhost:8000) in your browser.

The local server command is optional; it does not install dependencies or build the application.

## Using the application

1. Open **Owners** and add an owner.
2. Open **Pets** and register a pet, selecting its owner.
3. Use **Appointments** to schedule visits and change an appointment's status. Mark completed visits as **Completed**; the dashboard counts these as completed checkups.
4. Use **Medical records** to add dated diagnosis, treatment, or vaccination details for a pet.
5. Search for a pet by name from the Pets page. Use the **Delete** action to remove records; deletion requires confirmation.

Clinic records are stored in the browser profile that opens the application. They are not synchronized between browsers or devices. Clearing browser site data can remove saved records. This standalone application does not provide user accounts, centralized storage, or a backup service.

## Technologies and tools

- **HTML5** for application structure and forms.
- **CSS3** for styling and responsive layouts.
- **Vanilla JavaScript** for navigation, data entry, search, rendering, and record management.
- **Browser `localStorage`** for client-side persistence.

There is no frontend framework, backend, or external runtime dependency.

## Project structure

```text
animals-clinic/
├── .gitignore   # Git exclusions for generated, local, and sensitive files
├── README.md    # Project overview and usage instructions
└── index.html   # Complete application (HTML, CSS, and JavaScript)
```
