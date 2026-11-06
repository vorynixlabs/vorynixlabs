# Vorynix Labs

Building dependable developer tooling for software quality, test orchestration, and release confidence.

## Current focus

### TestForge Platform

TestForge is a software-testing operations platform focused on repeatable execution and explainable release decisions. Current work includes:

- deterministic parameterized test matrices
- run validation, scheduling, cancellation, and worker coordination
- retry governance and flaky-test classification
- accountable quarantine review workflows
- baseline comparisons and regression budgets
- report generation, artifact handling, and audit trails

The production repository remains private. The public
[testforge-platform-demo](https://github.com/vorynixlabs/testforge-platform-demo)
contains independently written, sanitized examples with tests and CI.

## Featured public project

### Artifact Guard

Artifact Guard is a zero-dependency Node.js tool for detecting credentials in
test logs and reports before CI uploads them. It combines explicit credential
rules with conservative entropy detection, returns masked findings, supports
JSON output and redaction, and uses CI-friendly exit codes.

```bash
git clone https://github.com/vorynixlabs/testforge-platform-demo.git
cd testforge-platform-demo
npm test
npm run scan:example
```

The example is tested on Node.js 20 and 22. Its fixtures are synthetic, and the
public repository contains no production source, private configuration, or
credentials.

## Engineering principles

- Prefer deterministic inputs and reproducible outputs.
- Preserve evidence behind every automated decision.
- Treat flaky tests as owned operational work, not hidden noise.
- Keep configuration validated, versioned, and reviewable.
- Use small focused changes with tests and CI verification.

## Active roadmap

- richer comparison dashboards and trend analysis
- quarantine ownership and review deadlines
- execution history and baseline persistence
- release-quality summaries for CI pipelines

## Repository activity

Public repositories contain runnable tools, architecture notes, and sanitized
examples. Ongoing platform implementation, pull requests, and CI validation
continue in the private TestForge repository.
