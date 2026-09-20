# Case study: PatchWitness SARIF reporting fix

Repository: [PatchWitness](https://github.com/pangxueyuan2-creator/patchwitness)

This is a maintainer-run case study from my own open-source project. It is not presented as a paid-client engagement.

## Problem

PatchWitness can reject a code change while still successfully completing its analysis and producing a report.

A SARIF export path incorrectly mapped a **rejected change** to `executionSuccessful: false`, which made "the gate rejected this change" look like "the analysis tool failed to run".

Those are different states and downstream tooling can care about the distinction.

## Before

For a valid failing Change Passport:

- the native gate result was **FAIL**
- the gate process correctly exited non-zero
- the SARIF report was produced
- but the SARIF invocation said `executionSuccessful: false`

That mixed up analysis completion with policy approval.

## Change

Pull request: [patchwitness#67](https://github.com/pangxueyuan2-creator/patchwitness/pull/67)

The fix:

- reports completed native analysis as `executionSuccessful: true`
- preserves the original failing gate status separately
- keeps gate exit behavior unchanged
- keeps findings, evidence digests, URI identity, and integrity behavior unchanged
- still rejects malformed, tampered, or unsupported native evidence

The important design rule was: **fix the reporting meaning without weakening the gate**.

## Verification evidence

The PR recorded verification on the exact proposed head, including:

- 36 focused reporter / path / CLI tests passing
- 549 collected local tests executed in disjoint groups
- hosted CI across Linux, macOS, and Windows
- Ruff, strict mypy, CLI smoke, package build / wheel smoke, and Docker smoke
- CodeQL, dependency review, and the repository's trusted-base self-gate
- an installed-wheel reproduction outside the checkout
- tamper and unsupported-status rejection checks

The PR also explicitly documented remaining limitations instead of calling the result "fully verified".

## Why this is representative

The useful part was not just editing one boolean.

The work required:

1. reproducing the semantic bug
2. identifying the trust boundary
3. making the smallest behavior change
4. protecting adjacent semantics with regression tests
5. validating the exact artifact that would be reviewed
6. writing down what was and was not proven

That is the kind of repository work I am comfortable taking on as a scoped engineering task.
