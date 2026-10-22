# GitHub Reading — AI-Bridge

Load `github-core.md` first.

Use this skill when checking discussion issue state, determining round completion, or deciding whether to update `topic_queue.md` or `synthesis_log.md`.

## Read Order for Discussion Issues

When inspecting a discussion issue, check in this order:

1. Issue open/closed state and title
2. Number of participant comments in Round 1 (expected: all non-presenter members)
3. Presenter response comment — present or absent
4. Number of participant comments in Round 2
5. Presenter final summary comment — present or absent
6. Whether the final summary includes a synthesis pattern

Do not assess round completion from comment count alone — read whether the right people posted.

## Round Completion Criteria

| Round | Complete when |
|---|---|
| Round 1 | All non-presenter participants have posted a feedback comment |
| Presenter response | Presenter has replied to Round 1 |
| Round 2 | All non-presenter participants have posted a follow-up comment |
| Session closed | Presenter final summary posted and issue closed |

If a participant is absent or has not posted within the expected window (3–5 days), note it explicitly — do not mark the round complete.

## What Counts as Meaningful Activity

Meaningful:
- A feedback comment from a named participant using the template structure
- A presenter response that addresses specific points
- A final summary with a concrete synthesis statement

Not sufficient by itself:
- Issue being open or closed
- A comment that only says "좋아요" or acknowledges receipt
- An LLM-generated draft not yet reviewed or confirmed by the participant

## topic_queue.md Reconciliation

Before updating `discussions/topic_queue.md`:

- Confirm the linked issue exists and its state matches the intended status change.
- `scheduled` → `done` only after the session is closed (issue closed + final summary present).
- If a session was cancelled or postponed, update to `parked` with a note — do not silently leave as `scheduled`.

## synthesis_log.md Update Conditions

Add an entry to `discussions/synthesis_log.md` only when:

- A reusable communication pattern is explicitly identified in the presenter's final summary.
- The pattern has not already been captured in a prior entry.
- The pattern generalizes beyond the specific topic — it describes a recurring dry/wet interpretation gap or a reusable LLM intervention.

Do not add entries that summarize a single session without extractable pattern. Session-level detail belongs in the meeting notes, not the synthesis log.

## Reporting Back

Summaries to the user should include:

- Round completion status per participant
- Any missing responses and who owes them
- Whether topic_queue.md needs updating
- Whether a synthesis_log.md entry is warranted

Keep it short. Do not dump raw comment content unless asked.
