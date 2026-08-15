# 🛠️ Open-source tools for trustworthy AI-assisted development

Hi, I'm **xueyuan Pang**.

I build small, local-first tools that help make AI coding agent changes easier to **inspect**, **constrain**, and **verify** — without asking a model to judge itself.

> Focus: evidence over trust · policy before action · offline-first verification

---

## 🔥 Flagship

### [PatchWitness](https://github.com/pangxueyuan2-creator/patchwitness)
**Independent trust gate for AI coding agents**

Turns a change into a verifiable **Change Passport**:
- Scope verification against real Git diff
- Protected files & CI rules from trusted base
- Real test execution evidence (not claims)
- Dependency impact analysis
- Offline SHA-256 integrity

[![CI](https://github.com/pangxueyuan2-creator/patchwitness/actions/workflows/ci.yml/badge.svg)](https://github.com/pangxueyuan2-creator/patchwitness/actions)
[![Release](https://img.shields.io/github/v/release/pangxueyuan2-creator/patchwitness)](https://github.com/pangxueyuan2-creator/patchwitness/releases)
[![Marketplace](https://img.shields.io/badge/GitHub_Marketplace-PatchWitness_Gate-2f81f7?logo=github)](https://github.com/marketplace/actions/patchwitness-gate)
[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/pangxueyuan2-creator/patchwitness/blob/main/LICENSE)

---

## 📦 Other tools

| Project | What it does | Status |
| --- | --- | --- |
| [**GuardSpec**](https://github.com/pangxueyuan2-creator/guardspec) | Compile repository intent into enforceable agent boundaries | Active |
| [**RuleRelay**](https://github.com/pangxueyuan2-creator/rule-relay) | Explain & validate AI coding-agent instruction files | Active |
| [**TaskToPR**](https://github.com/pangxueyuan2-creator/tasktopr) | Turn a GitHub Issue into a transparent, tested Pull Request | Active |
| [**Repo Privacy Guard**](https://github.com/pangxueyuan2-creator/repo-privacy-guard) | Offline-first secret & privacy scanner before going public | Active |
| [**SheetSentry**](https://github.com/pangxueyuan2-creator/sheetsentry) | Local-first CSV/TSV inspection + formula-injection safe sanitization | Active |
| [**OSS README Studio**](https://github.com/pangxueyuan2-creator/oss-readme-studio) | Free, no-sign-in bilingual README generator | Active |

---

## 🧠 Approach

1. **Make intent explicit** before an agent acts  
2. **Collect independent evidence** while the change is made  
3. **Keep the review surface inspectable** without model self-judgment  

These are intentionally small tools, not a hosted platform.  
Each repo documents its own limitations and threat model.

---

## 📍 Status

Early stage · Single maintainer · No production adoption claims yet

I'm actively building and iterating. Feedback, issues, and PRs are welcome on any of the projects above.

---

*Building safer defaults for the age of AI coding agents.*
