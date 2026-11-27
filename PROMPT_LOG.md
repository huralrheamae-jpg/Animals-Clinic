# AI prompt log

This log records the prompts visible in this working session. The earlier starter entries were not verifiable records of prompts actually sent, so they have been removed. Add any prompts from previous sessions yourself before submitting; do not claim prompts or results that you cannot verify.

## Prompt 1 · Git push error

**Date:** 2026-11-27  
**Prompt (summary):** Fix the shown `git push` errors (`src refspec main/master does not match any`) for the Animals Clinic repository.  
**Work/result:** Checked the current checkout. It is on `main`, has commit history, and `main` matches `origin/main`, so the earlier error does not reproduce in this checkout. The likely cause was running the push from a different/uncommitted repository state. No force-push was used.

## Prompt 2 · Lab 1 app and deliverables

**Date:** 2026-11-27  
**Prompt (summary):** Adapt the project to the Lab 1 requirements: a community problem, one FR-01 feature, one HTML page with `localStorage`, README, one-page project brief, prompt log, and test table.  
**Work/result:** Replaced the multi-section clinic suite with the single-feature Pawcare Appointment Book, documented the problem as an assumption to verify, and added the required FR-01 and deliverables. Verified seven browser checks covering valid save, blank and whitespace-only input, past and invalid dates, refresh persistence, and markup-like input; results are in the README test table.
