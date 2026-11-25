# Email rules for {{USER_NAME}}

These rules are a living file. The hub adds a rule whenever {{USER_NAME}} corrects it, with the date.

## Noise: archive without asking
Archiving means removing the item from the inbox; read status is not changed. Noise is never deleted.

**Never treat as noise:** mail from a colleague at `{{COMPANY_DOMAIN}}`, approval requests, invoices, anything that mentions {{USER_NAME}}, or mail where {{USER_NAME}} is in To: and a person is waiting.

{{NOISE_RULES}}
<!-- Examples (keep, edit or delete):
- Social network notifications (digests, job alerts). Exception: newsletters on the "interesting" list below.
- SaaS marketing, drip campaigns and webinar invites older than 7 days.
- Event promos after the event date.
- Calendar RSVP and out-of-office replies (Accepted / Declined / Automatic reply).
- Document comment notifications older than 21 days (newer ones may be mentions).
- Security alerts older than 7 days.
- Copies of your own booking confirmations. Receipts only after the related expense report is filed.
- Clusters of cold-outreach domains with an identical template = one agency → noise.
-->

## Always in the brief
{{MUST_INCLUDE_RULES}}
<!-- Examples:
- Approvals: {{APPROVAL_TYPES}}.
- Mentions in tickets, wiki pages and document comments.
- A person writes directly to {{USER_NAME}} (To:, not just CC) and expects an answer.
- Work mail written by a person, where {{USER_NAME}} is among the recipients, even in a group of 15. At least one line in FYI. If it touches {{GOALS}} or {{USER_NAME}}'s people, it gets a 💡 card with a concrete suggested action. Content decides, not read status: people often read on the phone and leave mail in the inbox.
- Warnings that something will be deleted or expire (API keys, OAuth clients, domains, subscriptions).
-->

## Newsletters worth a 1–2 line extract
{{NEWSLETTERS}}

## Vendor pitches (cold outreach)
For each pitch, write one sentence: who it is, what they offer, and whether it is relevant (yes / no / maybe, and why).
- Relevant topics: {{VENDOR_RELEVANT_TOPICS}}
- Not relevant: {{VENDOR_IRRELEVANT_TOPICS}}
- Warm contacts, not pitches: {{WARM_VENDORS}}
- For promising pitches, offer `research N`. That means checking:
  - has the company already looked at this vendor (chat, wiki)?
  - references;
  - price.

## Draft replies
Write drafts in the style of `writing-style.md`. Create a draft only as a reply in its thread. **Never send** without {{USER_NAME}}'s click on that exact draft.
