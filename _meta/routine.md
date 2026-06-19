# Improvement routine

A standing process to gradually grow and maintain the whole KB, **one small bite at a time**. Every mode is governed by the **strict factuality gate** in `CLAUDE.md` — propose source-grounded edits, never publish (`public:`/`published:`) without the user's say-so, and report the source behind each factual claim.

Source list for the fetch-based modes lives in `_meta/sources.md`.

## One chunk per run (core principle)

Each run surfaces **exactly one digestible item** for review — not a sweep. A chunk is small enough to approve or reject in under a minute: one development on one project, one missing glossary term, one stub to expand, one set of links on one page. The reply is a single yes/no/tweak, then done. Frequency does the work that a big sweep would — many small passes, each trivially reviewable.

Pick the single highest-value chunk available, rotating modes so attention spreads across the KB rather than fixating on one corner. Present it as: **the proposed change, its source, and the one decision asked of the user.** Stop after one.

## Modes (each yields one chunk)

1. **updates** *(currency — the main event)*
   Check the city news/Civic Alerts feed and the CivicClerk portal (recent Council/Planning Commission agendas & minutes) for **the single newest development** touching a tracked project in `_meta/sources.md`. Propose one dated, source-linked edit to that page (or one new stub for a genuinely new matter). Bump `updated:`/`status:`.

2. **onboard** *(newcomer resources)*
   Propose **one** newcomer/civic-literacy item: a single glossary term (proffer, by-right, special use permit), or one short "how to" (speak at Council, read an agenda, how Smart Scale scoring works). Source-grounded via the city's own process pages. Evergreen, so it ages slowly.

3. **deepen** *(expand stubs)*
   Take **the single thinnest** tracked page (fewest lines/links) and propose one focused expansion from a source — a decision timeline, the responsible body, the history. Stay structural if no source is reachable.

4. **garden** *(structural maintenance)*
   One structural fix: add the `[[wikilinks]]` missing from **one** page, create **one** stub for an unresolved wikilink, connect **one** orphan, or normalize one page's headings/frontmatter. No new external facts required.

5. **freshness** *(staleness check)*
   Take the **single oldest** `status: active` page by `updated:` and re-check its source — confirm still-current (bump `updated:`) or surface the one thing that changed.

## Cadence

Small and frequent beats big and weekly. Run often — daily or a few times a week — each run delivering one chunk:

- Default rotation across runs: `updates` most often (matches the Council calendar), with `onboard` / `deepen` / `garden` / `freshness` cycling in between.
- Run interactively whenever via `/loop` (one chunk, review, done), or schedule a **daily** cloud agent via `/schedule` that surfaces one chunk and pings you for the single decision.

## Frontmatter for tracking

Tracked project/topic pages should carry, beyond `title:`/`date:`:

- `updated: YYYY-MM-DD` — last time the page was checked against a source.
- `status: active | monitoring | resolved` — so `freshness` knows what to re-check.
