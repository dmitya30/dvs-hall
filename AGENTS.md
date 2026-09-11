# AGENTS.md — Mandatory Execution Contract

This file is the first operational source of truth after dialogue compression or context restoration.

## Project

- Project: DVS Hall conversion landing page.
- Deliverable: a one-page landing page implemented on Tilda.
- Business area: supply of contract engines and related automotive parts to customers in Russia.
- Primary acquisition channels: Yandex Direct Search and Yandex Advertising Network.
- Conversion channels: telephone, Telegram, WhatsApp and MAX.
- Public lead forms are excluded unless the owner explicitly reopens that decision.
- Market demand, customer objections and advertising compliance take priority over unsupported seller preferences.
- The three client-supplied prior websites are the owner-approved commercial baseline. Their repeated claims may be used in the landing page unless the owner corrects them or a material contradiction appears.

## User environment

- Shell: Git Bash MINGW64 on Windows.
- Canonical local repository path: `~/projects/dvs-hall`.
- Repository: `https://github.com/dmitya30/dvs-hall`.
- The assistant writes commands and patches; Dmitry Panevin applies them.
- Every executable patch must begin with an explicit `cd ~/projects/dvs-hall`.
- Never use `exit`, `exit 1`, `set -e` or commands that close the active Git Bash session.

## Patch delivery format

- Deliver each operational patch as one complete executable code block.
- Do not split one operation across separately copied code blocks.
- Do not use heredoc syntax, including Python and `cat` heredocs.
- Avoid unfinished shell structures that can produce the secondary prompt.
- Prefer deterministic file replacements or narrowly scoped Python commands.
- On Windows Git Bash, never pass large source files, HTML documents or other long payloads through `python -c`. Write a temporary `.py` file, run it, validate the result and delete the temporary file only after successful validation.
- Read the actual repository state and file schema before modifying existing files.
- Do not invent paths, schemas, Tilda capabilities, business facts, contacts, legal details or analytics settings.
- Do not provide placeholder implementation when an executable patch is required.
- Tracked text files must end with exactly one newline and no additional blank line at EOF.
- Never use `git diff --check`, `git diff --cached --check` or trailing-whitespace warnings as validation or commit gates in this repository. Trailing whitespace in generated or embedded HTML is non-blocking and must not prevent commit or push.
- Before committing, mechanically verify the exact staged file list.
- Do not print full diffs from executable scripts. Diagnostic output is allowed when validation fails.
- Never overwrite unavailable uncommitted local work based on reconstructed memory.

## Research standard

- Treat statements from Dmitry and explicit owner decisions as authoritative project inputs. Distinguish them from independently verified market facts and competitor claims.
- Separate every material item into one of four classes: verified fact, source claim, hypothesis or project decision.
- For current market, legal, advertising-policy and platform claims, use current sources and record the URL and access date.
- Prefer primary sources for laws, Yandex policies, Tilda capabilities and official business information.
- Search demand and competitor conclusions require evidence; visual preference alone is not market validation.
- Do not treat competitor copy, reviews, counters or guarantees as true without independent evidence.
- Do not infer that absence of information proves a weakness.
- Record disagreements and unresolved evidence instead of silently choosing a convenient version.
- Never promise that Yandex will approve advertising. The project can reduce identifiable compliance risks but approval remains Yandex decision.
- Do not repeat completed research after context compression when its sources and conclusions are preserved in the repository.

## Landing-page principles

- Build from demand: query intent, audience segments, objections, trust requirements and desired contact action.
- Keep the page proportionate to the stated budget and deadline; do not expand it into a catalogue or multi-page website without approval.
- Do not use lead forms, quizzes, callback widgets or file-upload fields under the current decision.
- Do not add fake reviews, fake inventory, fake counters, fake offices, fake certificates or unverifiable urgency.
- Claims consistently present on the three client-supplied prior websites are approved for reuse as client-provided commercial claims. Do not strengthen, quantify or extend them beyond that baseline without approval.
- Phone and messenger links must not be published until final contacts are supplied and checked.
- Do not conceal the actual seller, substitute unrelated legal entities or create misleading identities for advertising approval.
- Ensure the landing page and advertisements describe the same offer without material contradictions.
- Minimize personal-data processing. Any analytics, cookies, call tracking or external widget must be documented and approved before publication.
- Do not assume that removing forms eliminates all personal-data or privacy obligations.

## Tilda implementation rules

- Current architecture decision: one Tilda page with one T123 HTML block containing namespaced semantic HTML, CSS and only essential JavaScript.
- Keep the canonical T123 source in the repository and paste the mechanically verified build into Tilda.
- Use a unique root class for every custom selector; do not style generic Tilda elements, universal selectors or bare HTML tags outside the root.
- The custom implementation must not depend on external JavaScript libraries, third-party page builders or monthly services.
- Validate custom code on a published technical URL because T123 code does not execute normally inside the Tilda editor.
- Confirm the client account, tariff, domain, page ownership and publishing access before implementation.
- Prefer native Tilda blocks when they meet the approved prototype; use Zero Block only where it materially improves the result.
- Keep custom code and external dependencies to the minimum needed.
- Verify mobile, tablet and desktop layouts before publication.
- Check all telephone and messenger links on a published test URL.
- Record integrations, custom code, fonts, analytics and domain settings in repository documentation.
- Do not enable analytics, cookies, forms, CRM integrations, call tracking or third-party widgets by default.
- Do not claim that a Tilda preview proves production-domain behavior.

## Gates

1. Repository and context baseline.
2. Existing-site and advertising-rejection audit.
3. Demand and competitor research.
4. Verified offer, seller identity, evidence and contact inventory.
5. Landing-page brief and information architecture.
6. Copy and claim review.
7. Tilda prototype.
8. Mobile, functional, privacy and advertising-compliance QA.
9. Human approval.
10. Publication and post-publication checks.

- Do not skip an earlier gate merely because the launch date is close.
- Do not publish before final contacts are supplied and the landing page is checked against the available Yandex moderation notice.
- Commit and push every mechanically validated implementation iteration immediately; never leave intended project changes only in the local working tree while waiting for visual QA.
- If visual QA finds defects, correct them in a subsequent commit. Visual QA gates control approval and publication, not whether validated work is versioned.
- Internal documentation may be committed after mechanical validation.

## Context restoration

1. Read `AGENTS.md`.
2. Read `docs/CONTEXT.md`.
3. Read only the research, decision or implementation document required for the immediate task.
4. Verify current Git HEAD and working-tree state before modifying files.
5. Continue from the latest recorded gate without reconstructing unavailable local work.

## Documentation language

- Owner-facing conclusions and briefs are written in Russian.
- Internal source registers may use English field labels where useful.
- State the document language in the header of a new owner-facing document.
- Do not hard-wrap prose in owner-facing documents; use one physical line per paragraph or list item.
- Keep prompts, headlines, button labels and advertising text on one physical line unless the interface itself requires otherwise.

## Roles

- Dmitry Panevin: developer and repository operator.
- Alexander Romanov: partner and lead manager for the project.
- Client identity and contracting seller: not yet verified.
