# Playbooks: do as much as possible before {{USER_NAME}} looks

Rule: before an item reaches the brief, **prepare** every item where {{USER_NAME}} has to decide or respond:
1. gather the facts;
2. check them;
3. write a 1–2 sentence verdict;
4. ready the recommended action (a draft, a text, an open page).

{{USER_NAME}} should only need to click. When unsure, say so openly ("not sure because …, please check").

Each verdict carries one of three marks:
- ✅ **looks fine / I recommend approving**, with the reason (concrete numbers, sources);
- ⚠️ **something's off / I suggest a change**, with what exactly is off and a ready fix (draft message, corrected text);
- ❓ **not sure**, with what is missing and what {{USER_NAME}} should check.

## Approvals ({{APPROVAL_TYPES}})
<!-- Write one subsection per approval type that the user handles. A generic pattern: -->
### Invoice from a contractor (example)
1. From the email or invoice tool, take the amount, period, reference number and cost center.
2. Compare it with the agreed basis: hours × rate (from `{{RATE_SOURCE}}`), plus agreed extras.
3. Compare the hours with the time-tracking tool. Are they approved?
4. Verdict:
   - **✅ it matches.** Recommended action: "Approve for me", only if enabled in {{ON_BEHALF_APPROVALS}}. Otherwise: "Open the approval page".
   - **⚠️ it doesn't match.** Name the exact difference and draft a short message to the contractor. Don't send it without a click.
   - **❓ data is missing.** Name what is missing, for example "hours not yet approved: approve them first?".

### Time-off / timesheet / access request (example)
Check:
- who it is (team, manager);
- whether it makes sense (for access: do they work in this area?);
- whether there are conflicts (team calendar, deadlines).

Give the verdict and the action.

## Texts to review (someone asks for feedback on a draft)
1. Open the full draft: the body, the attachment, or the doc.
2. Check facts (roles, numbers, names), tone, length, and whether it sounds like {{USER_NAME}}.
3. Verdict: ✅ "fine to approve", ⚠️ "suggested edits" (show the edited version), or ❓.
4. Prepare the reply to the sender as a draft.

## Vendor pitches
See `email-rules.md`. For "maybe relevant" ones, do mini-research before the brief:
- did the company already look at this (chat, wiki)?
- what exactly do they do, and for whom?
- what does it cost?

Verdict, plus a ready polite "no" or "forwarding to a colleague" draft.

## Questions to {{USER_NAME}} in chat or email
Find the context: the thread, tickets, earlier answers. Propose a reply in {{USER_NAME}}'s style as ready text. Verdict = "I suggest replying like this".

## Meeting prep
For each meeting today where {{USER_NAME}} discusses something (1:1, review, steering; not all-hands, trainings or blocked time), prepare "what to discuss":
1. **{{USER_NAME}}'s own notes** for that meeting (mapping in `meetings.md`). Topics {{USER_NAME}} wrote at the top go first. From the last 2–3 entries, pick unfinished things (open checkboxes, "will…", open questions) and check whether they moved since.
2. **What's happening now:**
   - chat with the participants and mentions over the last ~14 days;
   - their tickets that are at risk or overdue;
   - tasks where the person or topic appears;
   - the invite's agenda;
   - open action items for that person (`state.json › meeting_followups`).
3. **Output:** 3–6 points, most urgent first. Each point gets 1–2 sentences on why now and a link. Order: {{USER_NAME}}'s own topics → decisions waiting → risks → open items from last time → "only if time allows". Say so when the notes are empty or recent meetings were cancelled.
4. **Writing prep into the notes page:** {{MEETING_NOTES_WRITE_POLICY}}
   <!-- Safe default: only after a click. Add a new dated block at the very top and change nothing else. Before writing, note the page version and the number of dated blocks. Afterwards, verify version +1, blocks +1 and old content intact. If anything is wrong, restore the previous content and tell {{USER_NAME}}. -->

## Deadlines from the task list
If it's work you can start (analysis, background doc, first draft), make a first version in a **side session** and put "ready, please review" with a link in the brief. If not, write the first step and what you need for it.

## Optional: performance notes for direct reports
<!-- Off by default. Some managers keep private notes per direct report. If enabled, the assistant may suggest a "Performance: suggested additions" idea card. Each observation is one specific situation with a date and a link, never a general judgment. Write to the notes page only after a click. Never mention these observations anywhere else. -->
{{PERFORMANCE_NOTES_POLICY}}
