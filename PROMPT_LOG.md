# Copilot Prompt Log

**Project:** Pawcare – Community Pet Appointment Tracker
**Date:** November 27, 2026

This document records prompts sent to GitHub Copilot while developing the Pawcare project. It also provides space to document Copilot's actual responses and the changes accepted.

Only include prompts actually sent to Copilot. Do not invent responses, changes, test results, or completed activities.

---

## Prompt 1 – Pawcare App Requirements

**Date:** 2026-11-27

**Prompt (verbatim opening):**

> I am a beginner web development student working on my Lab 1 project. I already have an existing Pawcare Clinic HTML project. I want you to help me improve and simplify it into a one-page web application called **Pawcare – Community Pet Appointment Tracker**.

The same message also specified the app purpose and the FR-01, validation, localStorage, design, scope, and verification requirements.

**Copilot's actual response:**

> [Paste or summarize the response you actually received.]

**Changes I made or accepted:**

- [Record what you actually changed or accepted.]

## Prompt 2 – FR-01 Review

**Date:** 2026-11-27

**Prompt (verbatim):**

> Review my Pawcare Appointment Tracker against the FR-01 requirements. Test all important functions, including adding appointments, required-field validation, rejecting past dates, updating status, deleting appointments, and localStorage persistence after refreshing. Fix any problems you find. Do not add new features. Explain each bug you fixed in beginner-friendly language.

**Copilot's actual response:**

> [Paste or summarize the response you actually received.]

**Changes I made or accepted:**

- [Record what you actually changed or accepted.]

## Prompt 3 – Visual Design Improvement

**Date:** 2026-11-27

**Prompt (verbatim):**

> Improve the visual design of my Pawcare Appointment Tracker while keeping the existing green-and-white Pawcare theme. Make the page responsive, clean, modern, and easy to use. Ensure that buttons, forms, tables, and messages do not overlap or hide important text. Do not change the FR-01 functionality or remove working features.

**Copilot's actual response:**

> [Paste or summarize the response you actually received.]

**Changes I made or accepted:**

- [Record what you actually changed or accepted.]

---

## Prompt 4 – Gradient Color

**Date:** 2026-11-27

**Prompt (verbatim):**

> add a nice gradient color

**Copilot's actual response:**

> [Add Copilot's actual response.]

**Changes I made or accepted:**

- [Describe the gradient changes made or accepted.]

---

## Prompt 5 – Project Documentation

**Date:** 2026-11-27

**Prompt (verbatim):**

> Help me prepare the documentation for my Pawcare Appointment Tracker Lab 1 project. Create or update README.md, PROJECT_BRIEF.md, and PROMPT_LOG.md. Explain the community problem, target users, FR-01, features, technologies, and localStorage architecture. In PROMPT_LOG.md, include only prompts actually used in this project and leave space for me to record Copilot's actual responses and changes. Do not invent completed tests, commits, or project activities.

**Copilot's actual response:**

> [Add Copilot's actual response.]

**Changes I made or accepted:**

- [Describe the documentation changes made or accepted.]

---

## Prompt 6 – Prompt Log Review

**Date:** 2026-11-27

**Prompt (verbatim):**

> check my PROMPT_LOG.md

**Copilot's actual response:**

> [Paste or summarize the response you actually received.]

**Changes I made or accepted:**

- [Describe the actual corrections made or accepted.]

---

## Prompt 7 – Lab 1 Requirements Verification

**Date:** 2026-11-27

**Prompt (verbatim):**

> I have completed the first version of my Pawcare – Community Pet Appointment Tracker. Please inspect my current index.html and verify that it meets my Lab 1 requirements.
>
> Do not redesign or rewrite the entire application.
>
> Please:
> 1. Check all appointment form fields.
> 2. Check that blank and whitespace-only required fields are rejected.
> 3. Check that past appointment dates are rejected.
> 4. Check that valid appointments can be saved.
> 5. Check that appointments remain after refreshing the browser.
> 6. Check that appointment status can be updated.
> 7. Check that appointments can be edited and deleted.
> 8. Check that localStorage is updated after every change.
> 9. Check that the design works on desktop and mobile.
> 10. Fix only actual bugs you find.
>
> After reviewing, give me a report with requirements that passed, problems found, changes made, and tests I still need to perform manually. Do not claim that browser tests passed unless you actually performed them.

**Copilot's actual response:**

> Browser-tested the requested core flows using fictional data. Required-field validation, past-date rejection, saving and refresh persistence, status changes, editing, deletion, and responsive layout checks passed. No application bug was found; the empty state after deleting the last appointment still needs a manual check.

**Changes I made or accepted:**

- [Record the actual fixes or changes accepted after reviewing the Copilot session.]

---

## Prompt 8 – Project Structure Inspection

**Date:** 2026-11-27

**Prompt (verbatim):**

> I am a beginner web development student working on my Lab 1 project called Pawcare – Community Pet Appointment Tracker.
>
> Please inspect my existing project files and explain the current structure. Do not delete or rewrite anything yet. Tell me what needs improvement to meet my Lab 1 requirements.

**Copilot's actual response:**

> Copilot inspected the app, documentation, `.gitignore`, and Git status. It reported the app structure and identified submission follow-ups: confirm the repository is public, verify the pull request, create the v0.1.0 release, add the YouTube demo link, and confirm the community problem with a clinic staff member.

**Changes I made or accepted:**

- [Record any actual changes made after the inspection.]

---

## Prompt 9 – Lab 1 Submission Preparation

**Date:** 2026-11-27

**Prompt (verbatim):**

> Thank you for inspecting my Pawcare project.
>
> Please help me prepare it for Lab 1 submission.
>
> Do not redesign or rewrite my application.
>
> 1. Review the current changes in index.html, README.md, PROJECT_BRIEF.md, and PROMPT_LOG.md.
> 2. Check whether README.md incorrectly claims that tests passed when they have not been performed.
> 3. Update the README test table so that untested cases are clearly marked "Not yet tested".
> 4. Review PROMPT_LOG.md and make sure it includes only prompts I actually sent to GitHub Copilot, including this inspection prompt.
> 5. Do not invent Copilot responses, test results, commits, pull requests, or releases.
> 6. Show me the Git changes before committing anything.
> 7. Give me a simple manual testing checklist for the application.
> 8. Explain how I can safely create and merge my pull request and create the v0.1.0 release.
>
> Do not commit, push, merge, or create a release without my permission.

**Copilot's actual response:**

> Copilot reviewed the project changes, updated the README test table to separate the tested deletion case from the untested empty-state case, and updated PROMPT_LOG.md. It reported that `git diff --check` was clean. It did not commit, push, merge, or create a release.

**Changes I made or accepted:**

- The README test table marks the last-appointment empty-state test as "Not yet tested".
- PROMPT_LOG.md was updated with additional actual prompt entries.
- No Git publishing actions were performed.

---

## Final Notes

- Use only fictional pet and owner information when testing the application.
- Fill in any remaining Copilot response and change fields using the actual Copilot Chat history.
- Do not mark tests as passed unless they were actually performed.
- Do not claim a pull request was merged or a release was published unless it was completed and verified.
- Keep this log updated when additional Copilot prompts are used.
