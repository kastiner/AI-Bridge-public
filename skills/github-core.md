# GitHub Core — AI-Bridge

Applies to all GitHub work in the AI-Bridge repo. GitHub here is the async communication layer between dry-lab and wet-lab researchers — not a code review platform.

## Purpose

Keep GitHub interactions structured, perspective-labeled, and useful for interdisciplinary synthesis. The goal is not just to record activity but to make interpretation differences visible and traceable over time.

## Core Principles

1. Read before write. Check issue state before posting or updating local files.
2. Always label perspective. When summarizing or translating, make explicit whose viewpoint is being represented (dry-lab / wet-lab / LLM synthesis).
3. Prefer structured posts over narrative dumps. The discussion templates exist for a reason — use them.
4. Do not infer round completion from issue state alone. Read the comments.
5. Keep posts purposeful. Every comment should either advance the discussion, clarify a gap, or close an action item.

## Tone

- Concise and factual.
- Perspective-neutral when synthesizing — do not collapse disagreement prematurely.
- If two disciplines interpreted the same result differently, report both views clearly before any synthesis.
- No filler, no praise, no redundant recap of what was already in the issue body.

## Verification Before Local Updates

Before updating `discussions/topic_queue.md` or `discussions/synthesis_log.md` based on GitHub state:

- Confirm the issue is actually closed or rounds are complete — not just that a comment exists.
- Read the latest meaningful comments, not just the issue metadata.
- Confirm the synthesis pattern is genuinely reusable, not session-specific noise.

If verification is incomplete, say so. Do not over-update local tracking.

## Tool Routing

1. Use the environment's supported GitHub connector or MCP integration for structured reads and writes.
2. Use `gh` CLI as a fallback when it is installed and authenticated.
3. Use local `git` only for file and branch operations.
4. Do not assume that a UI status such as `Connected` proves repository access; verify with a real read.

## Public-Action Safety

Before posting any comment or filing any issue:

- Confirm the content matches the current discussion round.
- Keep posts scoped — one purpose per comment.
- Do not post LLM-generated summaries as if they represent a participant's view. Label them explicitly as LLM synthesis.
- Do not close issues or mark rounds complete without verifying all participants have responded.
