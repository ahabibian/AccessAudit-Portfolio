# Engineering Highlights

## 1. Scanner Adapter, Not Scanner Product

The architecture does not couple the product identity to one scanning engine. Scanner output enters through an adapter boundary and becomes structured evidence for downstream workflows.

## 2. Evidence Integrity

Accessibility findings retain technical context needed for engineering review. Customer-facing presentation is derived from canonical evidence rather than replacing it.

## 3. Confirmed vs Manual Review

The system treats uncertainty as a first-class state. Findings that require human assessment are not converted into false automated certainty.

## 4. Deterministic Customer Reporting

Professional PDF output is generated from canonical report data through deterministic presentation rules. Material presentation-policy changes are versioned.

## 5. Representative Evidence Without Misleading Counts

The report can show a small number of useful examples while still displaying the true number of affected elements. Representative selection is deterministic rather than arbitrary.

## 6. Technical and Executive Layers

The reporting model separates stakeholder-oriented summaries from customer findings and developer-level technical evidence. This avoids forcing one document layer to serve incompatible audiences.

## 7. Browser-Rendered PDF Validation

The production reporting workflow has been validated with real Chromium PDF generation and visual inspection, including regression coverage for page flow, long evidence, contrast handling, and appendix pagination.

## 8. Accessibility-Specific Truthfulness

The system avoids overstating what automation can prove. Manual review, uncertain contrast measurement, source evidence, and canonical finding state remain explicitly represented.

## 9. Validation Depth

Recent private-repository validation has included:

- 1,700+ passing tests,
- 2,000+ subtests,
- focused PDF regression suites,
- canonical compatibility checks,
- GitHub Actions validation,
- Python compilation checks,
- real PDF rendering and page-by-page visual review.

These figures are engineering context rather than a substitute for architectural quality.

## 10. Product Lifecycle Beyond Detection

The product boundary extends beyond issue detection into review, remediation, re-scan, comparison, and reporting. This makes the system closer to an accessibility compliance workflow than a scanner wrapper.
