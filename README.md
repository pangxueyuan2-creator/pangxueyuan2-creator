# xueyuan Pang

I write small local tools that try to keep AI coding agents from quietly messing things up.

Mostly offline-first. No accounts, no dashboard, no "platform". Just something you can run and actually look at the output of.

---

**[PatchWitness](https://github.com/pangxueyuan2-creator/patchwitness)**  
Main project. Takes a code change and produces a Change Passport — what was touched, whether protected paths or CI got modified, whether the tests actually ran, and a hash you can verify later. Useful when you don't want to just trust the summary the model gave you.

---

Other things I've been working on:

- **[GuardSpec](https://github.com/pangxueyuan2-creator/guardspec)** — turns the rules people put in AGENTS.md / CLAUDE.md / Cursor rules into something you can check against before an agent runs
- **[RuleRelay](https://github.com/pangxueyuan2-creator/rule-relay)** — finds and explains those agent instruction files in a repo
- **[TaskToPR](https://github.com/pangxueyuan2-creator/tasktopr)** — takes one GitHub Issue, makes a small change on a branch, runs the tests, optionally opens a PR. Leaves an evidence folder behind
- **[Repo Privacy Guard](https://github.com/pangxueyuan2-creator/repo-privacy-guard)** — offline scanner for secrets and privacy issues before you make a repo public
- **[SheetSentry](https://github.com/pangxueyuan2-creator/sheetsentry)** — local CSV/TSV checker that also looks for formula injection problems
- **[OSS README Studio](https://github.com/pangxueyuan2-creator/oss-readme-studio)** — free bilingual README generator, no sign-up needed

---

Still early. One person. Every repo has its own limitations written down.

If any of this is useful, issues and PRs are welcome.
