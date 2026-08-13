# Open-source tooling for trustworthy AI-assisted software delivery

I build **local-first developer tools** that help teams make AI-assisted changes easier to inspect, constrain, verify, and share. The projects here focus on deterministic policy checks, change evidence, safe repository automation, and privacy-aware developer workflows.

## Featured projects

| Project | What it does | Best starting point |
| --- | --- | --- |
| [PatchWitness](https://github.com/pangxueyuan2-creator/patchwitness) | Produces a verifiable Change Passport for a patch: scope, protected files, executed checks, secret findings, dependency impact, and portable evidence. | Run the [60-second demo](https://github.com/pangxueyuan2-creator/patchwitness#60-second-demo-tests-pass-the-gate-fails). |
| [GuardSpec](https://github.com/pangxueyuan2-creator/guardspec) | Compiles explicit repository instructions into deterministic, reviewable boundaries for paths, commands, network domains, and MCP servers. | Try its [quick start](https://github.com/pangxueyuan2-creator/guardspec#quick-start). |
| [TaskToPR](https://github.com/pangxueyuan2-creator/tasktopr) | Turns one GitHub Issue into a bounded, tested, reviewable local change or Pull Request. | Run the [repeatable demo](https://github.com/pangxueyuan2-creator/tasktopr#repeatable-60-second-demo). |
| [SheetSentry](https://github.com/pangxueyuan2-creator/sheetsentry) | Inspects and safely sanitizes CSV/TSV data locally before it is shared or imported. | Read the [README](https://github.com/pangxueyuan2-creator/sheetsentry). |
| [Repo Privacy Guard](https://github.com/pangxueyuan2-creator/repo-privacy-guard) | Scans a repository for secrets and privacy-sensitive material before it becomes public. | Review the [scanner workflow](https://github.com/pangxueyuan2-creator/repo-privacy-guard). |
| [OSS README Studio](https://github.com/pangxueyuan2-creator/oss-readme-studio) | A free, no-sign-in bilingual README generator and quality audit for open-source maintainers. | Open the [public demo](https://pangxueyuan2-creator.github.io/oss-readme-studio/). |

## A practical trust boundary

> **Make repository intent explicit before work begins, preserve evidence while a change is made, and keep the resulting review surface inspectable without relying on a model to judge itself.**

The projects are intentionally small, composable tools rather than a hosted control plane. Each repository documents its own threat model, limitations, and supported workflows. In particular, a passing check is evidence of the checks actually performed—not a claim of semantic correctness.

| Stage | Useful project | Question it helps answer |
| --- | --- | --- |
| Before an agent acts | [GuardSpec](https://github.com/pangxueyuan2-creator/guardspec) | Which explicit repository boundaries apply to this task? |
| During a bounded repair | [TaskToPR](https://github.com/pangxueyuan2-creator/tasktopr) | Can this issue be turned into a transparent, tested change? |
| Before merge | [PatchWitness](https://github.com/pangxueyuan2-creator/patchwitness) | What independently collected evidence supports this patch? |
| Before sharing a repository or data file | [Repo Privacy Guard](https://github.com/pangxueyuan2-creator/repo-privacy-guard) and [SheetSentry](https://github.com/pangxueyuan2-creator/sheetsentry) | Could this material expose a secret, sensitive field, or unsafe spreadsheet formula? |

## Explore and contribute

Each project includes its own installation, security, and contribution guidance. For small, well-scoped contributions, start with repositories that label a task as [`good first issue`](https://github.com/search?q=user%3Apangxueyuan2-creator+label%3A%22good+first+issue%22+state%3Aopen&type=issues). Please use a repository's `SECURITY.md` rather than a public issue for a potential vulnerability.

This profile intentionally avoids vanity metrics and unsupported claims. The source repositories, demonstrations, test suites, release notes, and limitations are the primary record of current project capabilities.
