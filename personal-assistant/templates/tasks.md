# Task list: how to read and write it

Tool: **{{TASK_TOOL_NAME}}**. Access method: {{TASK_ACCESS_METHOD}} (connector / API / browser / local file).

## Format of a task
- Text starts with the label: `L · `, `N · ` or `O · `.
- With a deadline, the date comes first: `Due {{DATE_EXAMPLE}} – L · …`.
- Each task ends with a link to its source, as a real hyperlink under a short word: "mail", "chat", "ticket", "notes".
- New tasks without a deadline go at the top. Tasks with a deadline go after the last task with an earlier deadline.

## Reading
Pick open (unchecked) tasks that are:
- due in the next 7 days or overdue;
- in progress ({{IN_PROGRESS_MARKER}});
- at the top of the list ({{USER_NAME}} sorts by importance).

## Writing
- After writing, read it back to verify: right position, right format, nothing else changed. If not, undo.
- **Never delete or reorder other tasks.**
- Done tasks: tick them off ({{DONE_HANDLING}}).
- Dropped tasks: tick off and add the sub-note "dropped <date>".
- If the tool needs a login, don't log in. Put a card in the brief: "please log in to {{TASK_TOOL_NAME}}". Keep pending tasks in `state.json › pending_notes` so nothing is lost.

{{TOOL_SPECIFIC_NOTES}}

<!--
### Option: a local file (simplest)
If the user has no task app, keep `{{ASSISTANT_DIR}}/TASKS.md`:
- `## Open` and `## Done` sections;
- one `- [ ]` line per task;
- sub-bullets for notes.
It is always reachable, versionable and readable on the phone through any file app.

### Option: a note in a notes app through the browser
Read with page text. Write only by inserting after the end of an existing item, never by replacing the note body: scripting APIs often rewrite the whole note and destroy checklists and links. Zoom in to verify formatting after each write.
-->
