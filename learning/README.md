# Learning Directory

Use this folder for process notes, search tactics, dead ends, and short lessons learned during the assignment.

## Purpose

- Keep working notes separate from research outputs
- Capture what worked and what did not
- Make it easier to repeat useful collection methods later

## Challenges Faced

- Some experts did not have an active or reachable YouTube channel, so full transcript collection was not possible for every source.
- A few YouTube videos had public pages but still blocked clean transcript extraction in this workspace.
- Supadata was enabled in Cursor, but it was not available as a usable MCP tool in this Codex workspace, so we could not rely on it here.
- Some public sources were accessible only as partial page text, not as a clean full post or transcript.
- The repo became hard to scan when the same platform was stored in different places and naming styles.

## How We Overcame the Challenges

- Used the CSV as the single source of truth for which links to collect.
- Kept fallback notes for blocked or partial-source cases instead of inventing missing content.
- Switched to other tools, including the browser and GitHub-hosted public page access, when Supadata MCP was not available in this workspace.
- Saved whatever public text was reachable, then labeled it clearly when it was incomplete.
- Reorganized the repository by platform, author, and newsletter so the structure stayed predictable.

## Approach

- Start from the spreadsheet and collect only the public links that are actually present.
- Organize outputs by platform first, then by author/newsletter inside each folder.
- Preserve verified public data even when the source is partial or blocked.
- Use GitHub and browser-based page access for public YouTube transcript collection when direct transcript tooling was unavailable.
- Keep process notes in `learning/` and research outputs in `research/`.

## Learning

- Real-world research is often partial, so the workflow needs clear fallback handling.
- A clean folder structure matters more than forcing every source into the same format.
- It is better to separate verified captures from incomplete notes than to blur them together.
- If one tool path fails, the workflow should still leave a usable trail by switching to another public-access method instead of stopping the collection entirely.
- Platform-by-platform organization makes the repo easier to maintain and explain.
