# EZERV MarginGuard

**Protect margins. Prevent losses. Retain customers. Grow profit.**

EZERV MarginGuard is a planned profitability and operations intelligence platform for retailers and small-to-medium businesses. It aims to connect sales, billing, inventory, procurement, expenses, and customer-service data to identify potential losses, explain their impact, and recommend practical, reviewable actions.

> **Project status:** This README is based on the project concept and proposed student MVP. Implementation and setup instructions will be added as the software is developed.

## What MarginGuard aims to do

- Calculate product, order, customer, supplier, and outlet profitability using clearly defined cost and tax assumptions.
- Flag billing exceptions, low-margin sales, excessive discounts, and unusual transactions for review.
- Track batches, expiry dates, slow-moving stock, and stock-out risk.
- Compare supplier quotations using landed cost, quality, delivery, minimum order quantities, and terms.
- Summarize expenses and identify unusual changes or budget variances.
- Provide demand or expiry-risk predictions with uncertainty and baseline comparisons.
- Answer business questions using approved platform data and create prioritized, auditable action items.
- Support customer service with respectful responses and prompt human handoff when requested or needed.

## Proposed student MVP

The initial release is intended to demonstrate a focused retail profitability workflow using a small dataset and simulated transactions:

1. Import or enter product, supplier, purchase, sales, and inventory data.
2. Calculate margins and flag billing or low-margin exceptions.
3. Track batches and expiry dates and show inventory at risk.
4. Summarize expenses and highlight simple anomalies or budget variances.
5. Compare supplier quotations for equivalent items using total value, not price alone.
6. Demonstrate a business copilot grounded in approved platform data.
7. Simulate customer cancellation/frustration detection and immediate human handoff.
8. Evaluate one predictive feature against a simple baseline.
9. Present prioritized actions, estimated impact, approvals, and audit history.

Full POS/accounting integrations, live supplier discovery, and advanced forecasting are later-phase possibilities, not MVP assumptions.

## Planned technology

| Area | Proposed tools |
| --- | --- |
| User interface | Streamlit for the student MVP |
| Application/API | Python; FastAPI is an option |
| Initial data import | CSV/Excel |
| Business calculations | Python, Pandas, and SQL |
| Predictive analytics | Scikit-learn or an appropriate forecasting library |
| Optimization and experiments | Suitable linear/mixed-integer or heuristic methods; SciPy, Statsmodels, and a DoCE library where justified |
| IoT | Simulated events first; MQTT/Mosquitto and ESP32 are optional |
| Database and reports | SQLite for the MVP; Plotly/Matplotlib and PDF/Excel exports as needed |

These are proposed choices, not a statement that the components are already implemented.

## Product principles and safeguards

- Make recommendations explainable, evidence-based, prioritized, and subject to owner approval.
- Never silently alter a financial transaction; preserve review and audit history.
- Do not invent supplier prices, product equivalence, refunds, or business facts.
- Show assumptions behind margins, forecasts, and estimated financial impact.
- Customer-service automation must respect customer choice. If a person is requested, cancellation is raised, or a serious issue occurs, provide prompt human escalation.
- Do not obstruct account-deletion requests or create repetitive retention loops.
- Use authorized business and customer data, protect credentials, and apply appropriate access controls.

## Development status

The project plan proposes a 16-week student MVP, progressing from sample data and business rules through margin/billing checks, inventory and expense workflows, supplier comparison, customer handoff, one predictive feature, and integration. Detailed installation, configuration, and contribution instructions will be added when the corresponding code and project tooling are available.
