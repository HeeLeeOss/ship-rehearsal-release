---
title: Ship rehearsal release
license: CC0-1.0
lifecycle: ai-full
---

## Problem

The `github-release` recipe of the `ship` stage has never run against a real GitHub release. Its tests use fakes, so nobody yet knows which host GitHub redirects a release asset's public address to, or whether the fetched bytes match. The Hee-Lee Oss maintainers need to see one real release shipped and fetched back before any real publication.

## Beneficiary

The Hee-Lee Oss maintainers. This is an internal rehearsal with no outside beneficiary. The output is one tiny text file and a record of what happened, reached through this repository's releases.

## Scope

One text file, `dist/hello.txt`, for milestone M1. The milestone is read, covered and shipped as a GitHub release on this repository, and the release's asset is fetched back and compared.

## Non-goals

No real publication, no software and no content that anyone is meant to use. Nothing in this project is delivered to anyone.

## Acceptance criteria

| AC | Case | Required evidence |
|---|---|---|
| AC-01 | `dist/hello.txt` holds the line "rehearsal release" | The file at the tip of the default branch |

## Inputs and provenance

None
