# Test Execution & Defect Report
**Employee:** Kaleemuddin Mohammed

## Summary
- Total: 20
- Passed: 17
- Failed: 3
- Environment: deterministic local booking-workflow simulation

## Defects
### HB-DEF-001 — Same-day stay handling unclear
Severity: Medium. Expected: reject or clearly support day-use. Actual: booking accepted without explanation.

### HB-DEF-002 — Total price does not refresh after date change
Severity: High. Expected: recalculate total. Actual: old total remains.

### HB-DEF-003 — Retry can create duplicate reservation
Severity: Critical. Expected: retry is idempotent. Actual: second reservation ID generated.

## Recommendation
Fix duplicate reservation handling first, then retest date modification and same-day date logic.
