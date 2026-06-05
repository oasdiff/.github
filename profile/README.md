# oasdiff

**OpenAPI breaking-change detection for API teams.**

oasdiff is the open-source toolchain teams use to catch breaking changes in OpenAPI specs before they ship. Run it as a CLI, in CI via the GitHub Action, or use the hosted side-by-side review workflow at [oasdiff.com](https://www.oasdiff.com) to approve or reject each change with a commit-status check.

[![release](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/oasdiff/.github/main/badges/release.json)](https://github.com/oasdiff/oasdiff/releases)
[![stars](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/oasdiff/.github/main/badges/stars.json&logo=github)](https://github.com/oasdiff/oasdiff/stargazers)
[![contributors](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/oasdiff/.github/main/badges/contributors.json)](https://github.com/oasdiff/oasdiff/graphs/contributors)
[![release downloads](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/oasdiff/.github/main/badges/downloads.json)](https://github.com/oasdiff/oasdiff/releases)
[![docker pulls](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/oasdiff/.github/main/badges/docker-pulls.json)](https://hub.docker.com/r/tufin/oasdiff)
[![license](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/oasdiff/oasdiff/blob/main/LICENSE)

## What it does

- **Diff and changelog.** A precise, machine-readable diff between any two OpenAPI specs, plus a human-readable changelog.
- **Breaking-change checks.** A library of rules that flag changes likely to break API consumers.
- **PR annotations.** The [oasdiff GitHub Action](https://github.com/oasdiff/oasdiff-action) marks breaking changes inline on the changed lines, in the Files Changed tab.
- **Side-by-side review.** Open any spec pair at [oasdiff.com/diff](https://www.oasdiff.com/diff) for a visual review.
- **Validate.** Catch OpenAPI and JSON Schema violations standalone, no diff required.

## Quick start

Try it without installing:

```bash
docker run --rm -t tufin/oasdiff diff \
  https://raw.githubusercontent.com/oasdiff/oasdiff/main/data/openapi-test1.yaml \
  https://raw.githubusercontent.com/oasdiff/oasdiff/main/data/openapi-test5.yaml
```

Install:

```bash
brew install oasdiff                                                                # macOS
go install github.com/oasdiff/oasdiff@latest                                        # Go
curl -fsSL https://raw.githubusercontent.com/oasdiff/oasdiff/main/install.sh | sh   # macOS or Linux
```

Or paste two specs at [oasdiff.com/diff](https://www.oasdiff.com/diff).

## Repositories

| Repo | What it is |
|---|---|
| [oasdiff/oasdiff](https://github.com/oasdiff/oasdiff) | Core CLI and Go library |
| [oasdiff/oasdiff-action](https://github.com/oasdiff/oasdiff-action) | GitHub Action for pull-request CI |

## oasdiff Pro

For teams that need block-on-merge controls, approve / reject directly on the GitHub PR comment, and per-org policy: see [oasdiff Pro](https://www.oasdiff.com/pricing).

## Project health

- Apache-2.0 licensed
- Active development with regular tagged releases
- Used in CI by API teams across SaaS, fintech, dev-tools, and OSS

## Get in touch

- Documentation: [oasdiff.com/docs](https://www.oasdiff.com/docs)
- Support and partnerships: [info@oasdiff.com](mailto:info@oasdiff.com)
- Issues and feature requests: [github.com/oasdiff/oasdiff/issues](https://github.com/oasdiff/oasdiff/issues)
- Terms of service: [oasdiff.com/terms](https://www.oasdiff.com/terms)
- Privacy policy: [oasdiff.com/privacy](https://www.oasdiff.com/privacy)
