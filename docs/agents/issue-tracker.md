# Issue tracker: GitHub Issues

Issues live in the GitHub repo: `github.com/maplepy/mise-app`

Uses the `gh` CLI.

## Wayfinding operations

Used by `/wayfinder`.

- **Map**: a GitHub Issue labelled `wayfinder:map`, with child issues labelled `wayfinder:research`, `wayfinder:prototype`, `wayfinder:grilling`, or `wayfinder:task`.
- **Child ticket**: a GitHub Issue linked as a related issue to the map.
- **Blocking**: use GitHub's native "Blocked by" dependency issue links (requires Pro for private repos; public repos get it free).
- **Frontier**: open issues with no blocking dependencies.
- **Claim**: assign the issue to yourself via `gh issue edit <n> --assignee @me` before any work.
- **Resolve**: add a comment with the answer, close the issue, and add a context pointer to the map's "Decisions so far" comment.

## Creating a map

```bash
gh issue create --title "<title>" --body "<map body>" --label "wayfinder:map"
```

## Creating a ticket

```bash
gh issue create --title "<question title>" --body "## Question\n\n<question>" --label "wayfinder:<type>" --assignee @me
gh issue edit <map-n> --add-relationship "blocks" <ticket-n>
```
