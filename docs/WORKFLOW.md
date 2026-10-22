# AI-Bridge public workflow

This workflow supports structured communication between computational and experimental researchers. It is a reusable pattern, not evidence that every stage was completed in the original project.

## Recommended session flow

```text
Prepare → Meet → Record interpretation gaps → Review the record
        → Optional GitHub discussion → Confirm actions → Capture reusable lessons
```

## 1. Prepare

The presenter completes [`templates/presentation_template.md`](templates/presentation_template.md):

- State the research question.
- Define terms and measurement boundaries.
- Identify where the two disciplines may apply different standards.
- Remove private or unpublished material before sharing anything publicly.

An LLM may help summarize background or translate terminology, but the presenter remains responsible for accuracy.

## 2. Meet

Suggested 60-minute structure:

| Time | Activity |
|---|---|
| 0–15 min | Present the question, evidence, and interpretation |
| 15–35 min | Compare computational and experimental interpretations |
| 35–50 min | Clarify assumptions, measurements, and missing evidence |
| 50–58 min | Agree on actions and unresolved questions |
| 58–60 min | Confirm the record owner and review deadline |

Use [`templates/meeting_notes_template.md`](templates/meeting_notes_template.md) to record what was actually discussed.

## 3. Review before sharing

Before a note or discussion is made public:

1. Each attributed viewpoint is confirmed by the person or discipline it represents.
2. LLM-generated wording is labeled and reviewed.
3. Private data and identifying details are removed.
4. Observation, interpretation, and proposed action are kept separate.

## 4. Optional GitHub discussion

Use GitHub only when it lowers—not raises—the participation burden.

- Standard post-meeting discussion: [`templates/discussion_template.md`](templates/discussion_template.md)
- Document-led discussion without a live presentation: [`templates/seeded_discussion_template.md`](templates/seeded_discussion_template.md)

Recommended two-round structure:

1. Participants describe what they understood, what is missing, and what matters from their discipline.
2. The presenter responds; participants then propose concrete next actions.
3. The presenter closes with agreements, unresolved points, and owners.

If GitHub access or navigation prevents participation, stop forcing the platform. Continue the scientific discussion through an accessible channel and use GitHub only as a reviewed archive.

## 5. Capture a reusable lesson

Record a general lesson only when it extends beyond one meeting:

```text
Problem → intervention → observed result → reusable rule
```

Do not convert a single anecdote into a general effectiveness claim.

## Public-action rule

An assistant may prepare a draft, but a person must review and approve it before any public issue, comment, or repository change is posted.
