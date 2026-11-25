# Chat rules for {{USER_NAME}} ({{CHAT_TOOL_NAME}})

## Identity
- {{USER_NAME}}'s user id: `{{CHAT_USER_ID}}`
- Self-DM, where the "brief ready" ping goes: `{{NOTIFY_CHANNEL}}`
- Workspace: `{{CHAT_WORKSPACE}}`
- Permalink format: `{{CHAT_PERMALINK_FORMAT}}`
  <!-- Slack: https://<workspace>.slack.com/archives/<channel>/p<ts without the dot> -->

## What counts as a notification (each one becomes its own card)
- Every DM and group DM with a new message from someone else.
- Every mention of {{USER_NAME}}, including group mentions they belong to.
- Every new reply in a thread {{USER_NAME}} posted in.
- {{USER_NAME}}'s emoji reaction on the last message means handled: ✅ 👍 👌 🙏 ❤️. The exception is 👀, which means "looking at it" and stays open.

## Marking as read
{{CHAT_MARK_READ_METHOD}}
<!-- Chat APIs usually can't mark items as read. If a browser is allowed: open the channel or thread URL in its own tab, wait ~4 s, press Escape, close the tab. Write nothing and react to nothing. Otherwise: leave it as is. -->

## Watched channels
Order in the brief: Tier 1 → Tier 2 → Tier 3. Group DMs count as Tier 1.

### Tier 1: read everything relevant, top of the brief
Include every thread with a decision, a question to {{USER_NAME}}'s role, an incident, or numbers.

| Channel | ID | What it is | Why it matters |
|---|---|---|---|
{{TIER1_ROWS}}

### Tier 2: one line per channel, only if something happened
| Channel | ID | What it is | Note |
|---|---|---|---|
{{TIER2_ROWS}}

### Tier 3: big items only
{{TIER3_LIST}}

### Skip
{{SKIP_LIST}}
<!-- Typical: social channels, bot and alert channels (except unusual spikes), finished projects. -->

## Writing on chat
Follow `writing-style.md` › Chat. A reply to a specific message always goes into its thread.
