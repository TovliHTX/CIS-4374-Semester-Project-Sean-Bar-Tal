# Smart Parking Platform — Work Breakdown Structure (WBS)

WE ARE $oftware ¢orp. | September 4–December 4, 2026

| WBS | Work package / deliverable | Owner | Baseline window | Predecessor |
|---|---|---|---|---|
| 1.1 | Competitive analysis and project acquisition (Project Charter) | PM / PO/BA | Sep 4–11 | — |
| 1.2 | Stakeholder analysis, SRS, prioritized product backlog | PO/BA | Sep 4–11 | 1.1 (concurrent review) |
| 1.3 | Scope and requirements approval | PO/BA | Sep 11 | 1.1, 1.2 |
| 2.1 | Architecture, API/data design | Backend | Sep 14–25 | 1.3 |
| 2.2 | Accessible web/mobile design and operator workflows | UX/UI | Sep 14–25 | 1.3 |
| 2.3 | WBS, schedule, resource/cost, RACI, risk, communication and charters | PM | Sep 14–25 | 1.3 |
| 2.4 | Design and delivery plan approval | PM | Sep 25 | 2.1–2.3 |
| 3.1 | Accounts, authentication, vehicles, data foundation | Backend / Web / Mobile | Sep 28–Oct 9 | 2.4 |
| 3.2 | Map, search, filters, location details and availability | Mapping / Backend | Sep 28–Oct 9 | 2.4 |
| 3.3 | Reservations, payments, history, receipts, refunds | Backend / Payment | Oct 12–23 | 3.1–3.2 |
| 3.4 | Extensions, cancellation, directions, notifications | Backend / Mapping / Payment | Oct 12–23 | 3.1–3.2 |
| 3.5 | Operator dashboard, pricing, inventory, occupancy and reporting | Backend / Web | Oct 12–30 | 3.1–3.2 |
| 3.6 | Integration and development milestone | Backend | Oct 26–30 | 3.3–3.4; rolling integration with 3.5 |
| 4.1 | Functional, integration and regression testing | QA | Nov 2–13 | 3.6 |
| 4.2 | Performance, availability, reliability, security and accessibility tests | QA / DevOps | Nov 2–13 | 3.6 |
| 4.3 | Defect correction, regression and stakeholder acceptance | QA / PO/BA | Nov 16–20 | 4.1–4.2 |
| 5.1 | Release readiness, deployment configuration and runbooks | DevOps / PM | Nov 23–Dec 4 | 4.3 |
| 5.2 | Production deployment, monitoring and operations handover | DevOps | Dec 4 | 5.1 |
| 5.3 | Closure report and maintenance proposal; sponsor sign-off | PM | Nov 23–Dec 4 | 4.3; sign-off after 5.2 |

Project monitoring, change control, communication and risk reviews run throughout all phases. Dates are planned milestones from the charter, not claims of actual completion. The closure report's earlier completion dates are explicitly hypothetical actuals and do not replace this baseline.

The WBS groups work into five phases: initiation (1), design (2), development (3), testing (4), and release/closure (5). Development work package 3.6 overlaps 3.5 for rolling integration; its milestone requires 3.5 completion. Release readiness and handover occur in sequence on the final date.

## Sprint backlog coordination

The [Trello work board](https://trello.com/b/mksQWn9Z/cis-4374-project-work-board) is authoritative for execution status. Each actual work card identifies its sprint, functional owner and SRS traceability or acceptance criteria. Per-sprint summary cards link the individual tasks. Do not interpret assignment to a past baseline sprint as confirmation that the work was completed.

| Sprint | Goal and backlog themes | Exit evidence |
|---|---|---|
| 1 | Registration/login, vehicles, database, live map, availability, destination search, filters, parking details; web/mobile and security foundations | Customer can find suitable parking using a valid account and working data feed. |
| 2 | Reservations, payments, payment confirmation, modification/cancellation, refunds, history/receipts, extensions, directions, alerts and preferences | Core booking/payment workflow is demonstrable, including policy and failure cases. |
| 3 | Dashboard, inventory, pricing, occupancy, reports, web/mobile completion, security and system integration | Operator and customer workflows integrated and ready for formal testing. |
| 4 | Functional/regression, accessibility/browser, refresh/performance, transaction reliability and availability tests | Traceable QA results and prioritized defects. |
| 5 | Stakeholder acceptance, defect correction and regression review | Acceptance evidence, resolved or approved residual defects and readiness decision. |
| 6 | Release runbooks and monitoring, deployment, handover, closure and maintenance proposal | Authorization, handover record and closure approval. |

The pre-existing saved-payment-methods card is retained as an optional deferred item, subject to approved scope change. It does not expand the baseline SRS automatically.

## Final report assembly

The final report should include the required supporting plans, header, footer, table of contents and figure captions. Record sponsor/stakeholder decisions as pending until approved. The assignment instructions, Project Charter, SRS, Gantt chart and Trello board establish the scope and scheduling baseline.
