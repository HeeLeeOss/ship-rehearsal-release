---
title: Ship rehearsal release
riskTier: low
license: CC0-1.0
lifecycle: ai-full
beneficiary: Hee-Lee Oss maintainers (a ship rehearsal fixture; no public deliverable)
definitionOfShipped: A GitHub release on the project repository for the milestone; nothing is delivered to anyone.
reviewPolicy:
  humanCheckpoints: [spec, plan, ship]
milestones:
  - { id: M1, title: Rehearsal release, rows: [AC-01] }
definitionOfShippedRecipe:
  kind: github-release
  params:
    paths: [dist/]
---

## Summary

A throwaway project that exists once, to rehearse the `github-release` recipe of the `ship` stage against a real GitHub release. It holds one tiny text file, `dist/hello.txt`, so that its one milestone can be read, covered and shipped. It is a good deed only in that it proves the release path before any real publication; it has no outside beneficiary.

## Scope

In scope: `dist/hello.txt` for milestone M1, and one GitHub release on the project repository. Out of scope: any real publication, any software or content anyone is meant to use, and any other registry or host.

## Risk

Low. There is no personal data, no high-stakes advice, no outside beneficiary and no real deliverable. The licence is CC0-1.0 and the project's only input is one line of text written for the rehearsal. It carries no evaluators, because the sandbox half of the shipped-tree evaluation is not built, and a project that needs one cannot ship yet.

## Approach

The maintainer writes the file by hand on the donated lane and merges its pull request. The milestone then has one real coverage read, whose record is merged by a person. `hee-lee-oss ship` is run at a terminal, with a person typing the plan's digest. It publishes a release with the asset, fetches the asset back from GitHub's public address and compares the bytes, and records the release URL, the tag's commit and the host GitHub redirected the asset to.

## Definition of shipped

A GitHub release exists for the milestone, its asset fetched back from GitHub matches the bytes in the repository, and `SHIPPED.md` records it as a rehearsal. Nothing is delivered to anyone.
