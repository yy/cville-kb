---
title: MyCville public reports
date: 2026-09-27
updated: 2026-09-27
status: monitoring
tags: [process, transportation, service-requests, data]
---

The City's [service-request page](https://www.charlottesville.gov/666/Service-Request) links to the [PublicStuff interface for Charlottesville](https://iframe.publicstuff.com/#?client_id=1000141). Public reports can also be retrieved through the [requests-list endpoint](https://vc0.publicstuff.com/api/2.0/requests_list?client_id=1000141).

## API starting point

On September 27, 2026, a GET request to the endpoint above succeeded without authentication and returned 75 records in `response.requests`, each wrapped in a `request` object. Observed fields include `id`, `title`, `description`, `status`, `date_created`, `address`, `lat`, and `lon`. Some records include attachments.

This verifies one response, not a complete historical export. Pagination, filtering, and coverage still need checking. No API documentation or stability guarantee has been verified; inspect the public interface's browser Network panel to learn which requests it makes before building an integration.

## Street-safety use

Potential use: find existing reports near school routes and track their status alongside [[Topic/Traffic calming street-width analysis]]. Whether close-call reports appear in this public feed remains unverified; absence from the feed should not be treated as absence of a reported problem.

The response can include reporter identifiers and free-text personal details. Keep shared analysis focused on street issues and request IDs rather than reproducing reporter information.

## Sources

- [City service-request page](https://www.charlottesville.gov/666/Service-Request)—verified the link and Charlottesville client ID on September 27, 2026.
- [Public reports interface](https://iframe.publicstuff.com/#?client_id=1000141)
- [Requests-list API response](https://vc0.publicstuff.com/api/2.0/requests_list?client_id=1000141)—response structure and fields checked September 27, 2026.
