# My Scheduler — Sample Test Cases

These are proposed manual acceptance tests, not evidence that tests have already passed. Fill in **Actual result** and **Status** after running them on the current build.

| ID | Area | Steps / input | Expected result | Actual result | Status |
|---|---|---|---|---|---|
| TC-01 | Launch | Install and open app on a supported device | App opens without crash | — | Not run |
| TC-02 | Task validation | Try saving a task with required title blank | Clear validation; invalid task is not saved | — | Not run |
| TC-03 | Task persistence | Create a task, close app, reopen | Task remains visible | — | Not run |
| TC-04 | Task update | Edit a saved task and save | Updated values appear after reopening | — | Not run |
| TC-05 | Task completion | Mark a task complete, then reopen list | Completion state remains consistent | — | Not run |
| TC-06 | Timetable validation | Enter an end time earlier than start time | Invalid time range is rejected or corrected clearly | — | Not run |
| TC-07 | Attendance | Add attendance for a course/date | Correct course, date, and status are displayed | — | Not run |
| TC-08 | Attendance summary | Add known present/absent sample records | Summary matches the app's documented calculation | — | Not run |
| TC-09 | Offline operation | Enable airplane mode and use locally stored features | Features documented as offline continue to work | — | Not run |
| TC-10 | Empty state | Open a section with no records | Helpful empty state appears; no crash | — | Not run |
| TC-11 | Persistence integrity | Create, edit, and delete a record; relaunch | Each operation persists correctly | — | Not run |
| TC-12 | Notifications (if implemented) | Schedule a reminder and test permission granted/denied | Behavior matches permission state and app design | — | Not run |
| TC-13 | Semester analysis | Enter a small known dataset | Displayed totals/percentages match hand calculation | — | Not run |
| TC-14 | Privacy | Review logs, repository, and build config | No real student data or secrets are exposed | — | Not run |
| TC-15 | Clean build | Clone repository and follow README | Build succeeds from documented steps | — | Not run |

## Synthetic data notes

- `sample_attendance.csv` and `sample_tasks.json` contain fictional records.
- Field names are illustrative and may not match the app's import format.
- Do not import these files directly into production without adapting and validating the schema.
