# gh-security-findings
gh extension to list Dependabot and CodeQL findings

## Install

`gh extension install jecxjo/gh-security-findings`

## Usage

No args lists of all severity levels of both Dependabot and CodeQL. Otherwise, select the type of scan and an optional severity filter results.

```sh
$ gh security-findings dependabot medium
Fetching Dependbot findings...
---
1: Open Redirect in node-forge
  URL: https://github.com/example/project/security/dependabot/1
  Severity: medium
  Creation: 2024-01-01T00:00:00Z
  Updated: 2024-01-01T00:00:00Z
  CVSS: CVSS:3.1/AV:N/AC:L/PR:N/UI:R/S:C/C:L/I:L/A:N
  Score: 6.1
  
$ gh security-findings codeql
Fetching CodeQL findings...
---
2: Server-side request forger
  URL: https://github.com/example/project/security/code-scanning/2
  Severity: critical
  Creation: 2024-01-01T00:00:00Z
  Updated: 2024-01-01T00:00:00Z
  File: src/foo/bar.java:80

$
```
