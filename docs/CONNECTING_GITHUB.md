# Connecting an assistant to this public repository

This repository can be used as a low-risk connection test because it contains only sanitized public material.

## Success criterion

A connector is working only when the assistant can retrieve repository content—for example, the title of `README.md` or the list of open issues. A UI status such as `Connected` is not sufficient.

## Connector test

1. Connect your own GitHub account through the assistant's supported GitHub integration.
2. Ask the assistant to read this repository's `README.md`.
3. Ask it to list open issues in `<OWNER>/AI-Bridge-public`.
4. If write access is needed, ask for a draft issue first. Review it before posting.

## GitHub CLI fallback

If the environment supports GitHub CLI:

```bash
gh auth login
gh auth status
gh repo view <OWNER>/AI-Bridge-public
gh issue list --repo <OWNER>/AI-Bridge-public
```

Use browser/device authorization where available. Never paste a personal access token or password into a chat message.

## Public-repository caution

Public access solves visibility, not privacy. Do not copy private meeting notes, photographs, receipts, infrastructure instructions, or unpublished research into this repository merely to make them accessible to a connector.
