# Open-source tools for trustworthy AI-assisted development

I build small, local-first tools that help make AI coding agent changes easier to inspect, constrain, and verify.

## Main projects

| Project | What it does |
| --- | --- |
| [**PatchWitness**](https://github.com/pangxueyuan2-creator/patchwitness) | Turns a change into a verifiable Change Passport (scope, protected files, real test execution, dependency impact, offline evidence). |
| [GuardSpec](https://github.com/pangxueyuan2-creator/guardspec) | Compiles repository instructions into enforceable agent boundaries. |
| [RuleRelay](https://github.com/pangxueyuan2-creator/rule-relay) | Finds and validates AI coding-agent instruction files. |
| [TaskToPR](https://github.com/pangxueyuan2-creator/tasktopr) | Turns a GitHub Issue into a bounded, tested change. |
| [Repo Privacy Guard](https://github.com/pangxueyuan2-creator/repo-privacy-guard) | Offline secret and privacy scanner before a repo goes public. |
| [SheetSentry](https://github.com/pangxueyuan2-creator/sheetsentry) | Local CSV/TSV inspection and safe sanitization. |
| [OSS README Studio](https://github.com/pangxueyuan2-creator/oss-readme-studio) | Free bilingual README generator. |

## Approach

Make intent explicit before an agent acts.  
Collect independent evidence while the change is made.  
Keep the review surface inspectable without asking a model to judge itself.

These are intentionally small tools, not a hosted platform. Each repo has its own limitations and threat model documented.

## Status

Early stage. Single maintainer. No production adoption claims yet.
