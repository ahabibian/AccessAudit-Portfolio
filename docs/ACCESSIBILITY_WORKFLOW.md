# Accessibility Workflow

## 1. Scan

A target is evaluated through a scanner-adapter boundary. Automated results are inputs into the product, not the final compliance verdict.

## 2. Evidence

Raw findings are normalized into structured evidence so downstream review and reporting can use stable data rather than presentation-specific output.

Evidence may include selectors, HTML snippets, source failure summaries, technical checks, rule identifiers, related targets, and contrast data where available.

## 3. Review

Findings are separated into machine-confirmable issues and cases that require manual assessment.

This distinction is important for accessibility work because not every criterion can be reliably determined by automation alone.

## 4. Remediation

Structured findings are paired with remediation guidance so development teams can understand what should change and why.

The workflow keeps customer-facing explanation and technical source evidence conceptually separate.

## 5. Re-scan

After remediation, the target can be evaluated again. Re-scanning is part of the product lifecycle rather than an unrelated second audit.

## 6. Comparison

The architecture supports comparing accessibility state across scans so teams can distinguish resolved, persistent, and newly introduced issues.

## 7. Compliance Report

Canonical report data is transformed into a professional customer-facing PDF with three layers:

- Executive Summary
- Customer Findings
- Technical Appendix

The report is designed to serve both decision-makers and technical teams without duplicating every raw evidence instance in the main narrative.

## Why This Workflow Matters

A scanner can produce a list of issues. A compliance workflow must do more:

- preserve evidence,
- expose uncertainty,
- support human review,
- guide remediation,
- verify change,
- and communicate results clearly.

That broader lifecycle is the product boundary for AccessAudit.
