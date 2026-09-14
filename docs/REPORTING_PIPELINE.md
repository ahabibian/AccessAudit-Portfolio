# Professional Reporting Pipeline

## Purpose

AccessAudit's reporting layer is designed to turn canonical accessibility evidence into a professional customer-facing document without weakening or rewriting the underlying truth.

## Reporting Structure

The customer PDF is organized into three layers:

### Executive Summary
A decision-oriented overview for stakeholders who need the main risks, priorities, and recommended starting actions without reading every technical detail.

### Customer Findings
A concise finding-by-finding section using representative evidence examples rather than repeating every affected node.

### Technical Appendix
A deeper engineering section that preserves richer developer evidence for implementation and review.

## Canonical Truth vs Presentation

The canonical report remains authoritative.

The PDF presentation layer may:

- reorder content for readability within defined contracts,
- choose bounded representative examples,
- group related information,
- format evidence for A4 output.

It must not silently change:

- finding classification,
- affected-element counts,
- canonical evidence,
- legal/contextual meaning,
- remediation truth,
- source technical evidence.

## Representative Evidence

Large accessibility findings can affect many elements. Rendering every instance in the main report can produce repetitive and unreadable documents.

AccessAudit therefore uses deterministic representative-example selection while preserving truthful affected counts.

This creates a deliberate separation between:

- how many elements are actually affected,
- how many canonical examples are available,
- how many examples are selected for customer presentation.

## Manual Review

Manual-review findings remain visually and semantically distinct from confirmed issues.

The report does not invent numeric certainty where reliable automated measurement was unavailable.

## PDF Generation

The professional report is rendered through a Chromium-based pipeline.

Validation has included real browser PDF generation, A4 pagination review, long-selector and long-HTML wrapping, page-break regression tests, and page-by-page visual inspection.

## Deterministic Presentation

Material changes to deterministic presentation behavior are versioned so report output can be attributed to the presentation policy that produced it.

## Current Public Boundary

The production templates, renderer internals, canonical schema implementation, and proprietary source code remain private. This portfolio documents the engineering principles and system boundaries only.
