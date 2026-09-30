# Validation Notes

## Static checks
- `index.html` is self-contained: HTML, CSS, and JavaScript are in one file.
- No external JavaScript library is required.
- JavaScript syntax checked with `node --check`.
- Application has four SWOT quadrants, TOWS recommendations, action plan, nine BMC blocks, print/PDF, DOC export, local save, and reset.

## Formula checks

### Factor priority
For Importance = 5 and Urgency = 4:
`5 × 4 = 20/25`.

This is a prioritization heuristic only.

### Strategy priority
For Relevance = 5, Impact = 4, Feasibility = 4, Risk = 2:
- reverse risk = `6 − 2 = 4`
- mean = `(5 + 4 + 4 + 4) / 4 = 4.25`
- priority = `4.25 × 20 = 85/100`

### Evidence coverage
A strategy links exactly two SWOT factors:
- both have evidence: 100%
- one has evidence: 50%
- neither has evidence: 0%

Evidence coverage never changes the strategy score.

## Interpretation checks
- Automatic strategy wording only reuses factor statements entered by the user.
- BMC is not auto-filled with invented facts.
- Empty BMC blocks are reported as `Belum cukup data / belum diisi`.
- Strategy score is explicitly described as decision-support, not probability or prediction.
- Reset requires user confirmation and clears the browser's local storage for this app.
