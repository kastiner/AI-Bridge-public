# GitHub Writing — AI-Bridge

Load `github-core.md` first.

Use this skill when filing discussion issues, posting round comments, or producing LLM-assisted summaries for the async discussion workflow.

## Filing a Discussion Issue

Open one issue per presentation session. Title format:

```
[토론] YYYY-MM-DD — <주제 한 줄>
```

Example: `[토론] 2026-05-20 — 측정값 0의 분야별 해석 차이`

Issue body — two paths:

- **Standard (post-meeting):** paste the Round 1 section from `docs/templates/discussion_template.md`. Do not add preamble or re-summarize the presentation — participants were present.
- **Seeded discussion (no live meeting):** use `docs/templates/seeded_discussion_template.md`. The body substitutes for the presentation — include background, source material links, core claim, interpretation gap table, and discussion questions before the Round 1 instructions.

Label: none required for now. Add labels as the project defines them.

Assign: the presenter is the issue owner.

## Round 1 Comments (Participant Feedback)

Each participant posts one comment using the Round 1 block from `docs/templates/discussion_template.md`.

When assisting a participant:
- Fill in their perspective label (dry-lab / wet-lab) explicitly at the top of the comment.
- Do not merge perspectives. If you are drafting for one participant, stay in their frame.
- Keep each point to 1–2 sentences. Longer explanations belong in a follow-up if needed.

## Presenter Response Comment

After all Round 1 comments are in, the presenter posts a response using the presenter response block from the template.

When assisting:
- Summarize which points will be incorporated and which cannot — do not silently drop feedback.
- Flag unresolved disagreements explicitly. Do not smooth them over.

## Round 2 Comments (Follow-up Plan)

Each participant posts a Round 2 comment using the Round 2 block from the template.

When assisting:
- Focus on concrete next steps — analysis, experiment, or communication change.
- Include an explicit "LLM evaluation" entry: what was useful, what required human judgment.

## Presenter Final Summary Comment

Closes the issue. Should answer:
- What was agreed.
- What remains unresolved.
- What concrete actions follow.
- A 2–3 sentence synthesis pattern for `discussions/synthesis_log.md`.

## LLM-Assisted Writing Rules

When Claude drafts or assists with any GitHub comment:

- Label the output: prepend `> *LLM 초안 — 검토 후 수정하세요*` for comments drafted entirely by LLM.
- Do not present LLM synthesis as a participant's personal view.
- Perspective translation (dry → wet or wet → dry) is a valid LLM task — label it as such.
- Follow-up question generation is a valid LLM task — present as suggestions, not conclusions.

## Length Discipline

| Content | Limit |
|---|---|
| Issue title | One line, under 60 characters |
| Round comment | Under 400 words per participant |
| Presenter response | Under 300 words |
| Final summary comment | Under 250 words + synthesis sentence |
| LLM synthesis block | Under 150 words |

If a comment is running long, split the observation from the action item into separate bullet points rather than prose.
