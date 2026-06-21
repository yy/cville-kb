# cville-kb — working instructions

A community knowledge base about Charlottesville civic matters (governance, transportation, infrastructure, planning), kept as an Obsidian vault of interlinked Markdown pages. Human-facing content policy lives in `CONTRIBUTING.md`; this file governs how to edit the vault.

## Strict factuality gate (hard rule)

The goal is zero unverified facts in this vault. The failure mode is writing civic facts from training memory instead of from a source checked *this session* — plausible-but-wrong is exactly how errors slip into a community resource. Guard against it:

1. **Source-grounded or omitted.** Every concrete fact — dates, vote counts, dollar amounts, project names, official titles, who voted how, who said what, "the council approved…", "the study found…", "scheduled for…" — must trace to a source you actually read this session: the page itself, a URL you fetched, an Obsidian note you opened, or tool/API output. Authoritative sources here are the city website, meeting minutes/agendas, ordinances/budgets/resolutions, Smart Scale or VDOT documents, FOIA responses, and dated news articles. If you can't ground it, leave it out. A shorter, correct page beats a fuller, unverified one.
2. **Fetch to ground; don't recall to fill.** Before expanding a stub or writing a description, actively fetch the primary source and write only what it supports. Retrieve first, then write from what you read — never write from memory and backfill confirmation.
3. **No hedged guessing.** "Reportedly", "is believed to", "around 2021", "roughly $2M" when the basis is memory are tells that you're guessing. Cut the claim rather than hedge it.
4. **When you can't fetch, stay structural.** If no source is reachable (offline, paywall, thin page, ambiguous identity), fall back to source-free edits — normalizing wikilinks, headings, and frontmatter; wikilinking terms already present in the text; connecting orphans. These need no external facts. Leave the body sparse rather than inventing content.
5. **Recall ≠ reading.** A civic fact known only from training memory is unverified — omit it even if it seems obvious. Council compositions, project timelines, and dollar figures all drift; treat them as needing a fresh source every time.

In your summary to the user, state the source for each factual claim you added (e.g., "vote count per fetched council minutes"), or note that you stayed structural because no source was available.

## Conventions

- Pages are Markdown in an Obsidian vault. Use `[[wikilinks]]` for internal cross-references.
- Write each paragraph as a single soft-wrapped line — no hard line breaks within a sentence or paragraph (Obsidian convention).
- Include YAML frontmatter with at least `title` and `date`; tracked project/topic pages also carry `updated:` and `status:` (active / monitoring / resolved).
- Link to primary sources rather than hosting copies; summarize in your own words.
- See `CONTRIBUTING.md` for the full content, sourcing, and privacy policy.

## Disambiguation

When pages could collide on the same subject or place:

- **Name by the project/initiative, not the location** — a place hosts many efforts over time, so the title says what is done, not just where (e.g. `West Main / Ridge intersection reconfiguration`, not `West Main / Ridge`).
- **Qualify colliding titles** by their distinguishing attribute — program plus round/year, or scope (e.g. `… (Smart Scale)`, `… FY28`). For Smart Scale, the round is usually the cleanest qualifier.
- **Group by place with a `location:` frontmatter field** so projects at the same spot stay collectable regardless of differing titles.
- **Add a place/index hub page only once a location has 2–3+ distinct projects**, linking each project and back — don't create it preemptively.
- **Folders disambiguate by type** — the same name can live in `Organization/` (the entity) and `Project/` (the effort), as with Cville Food Co-op.

## Improvement routine

To grow and maintain the KB, run the modal routine in `_meta/routine.md` — **one small, reviewable chunk per run** (modes: `updates`, `onboard`, `deepen`, `garden`, `freshness`), starting from the verified source list in `_meta/sources.md`. Every mode is governed by the strict factuality gate above.
