# IT Service Desk Operations Report
**Period:** January – June 2024  s
**Prepared by:** Brahma Borude, Data Analyst  
**Audience:** IT Operations Director

---

## Executive Summary

| Metric | Value | Target | Status |
|--------|-------|--------|--------|
| SLA Compliance Rate | 76.8% | 90.0% | ❌ Below target |
| Overall MTTR | 23.0 hours | < 12h | ⚠️ Above target |
| P1-Critical Breach Rate | 30.4% | < 10% | ❌ Critical |
| Total Tickets Analysed | 5,000 | — | — |

---

## Finding 1 — SLA Compliance: 76.8% vs 90% Target

**Observation:** Overall SLA compliance is 76.8%, which is
13.2 percentage points below the 90% contract target.
P1-Critical tickets have the highest breach rate at 30.4%.

**Business impact:** P1 breaches represent system-down events affecting
multiple users. Continued breach rates above 30% risk contract
penalty clauses with service clients.

**Recommendation:** Implement auto-escalation for any P1 ticket unresolved
after 2 hours. Maintain senior engineer standby during 10PM–6AM window.

---

## Finding 2 — Agent Workload Imbalance

**Observation:** AGT-00001 handles 609
tickets vs team average of 333.
High-load agents show 29.3% breach rate vs
team average of 23.1%.

**Recommendation:** Cap individual queues at 1.2× team average.
Implement round-robin assignment for P3/P4 tickets.

---

## Finding 3 — MTTR Trend

**Observation:** Overall MTTR is 23.0 hours.
Best month: 21.8h avg. Worst month: 23.6h avg.
Highest-MTTR category: Access Management at 24.8% breach rate.

**Recommendation:** Set MTTR alert threshold at 28 hours.
Trigger resource review if exceeded for 2 consecutive weeks.

---

## Recommended Actions (Priority Order)

1. **P1 auto-escalation protocol** — implement within 2 weeks
2. **Rebalance agent queues** — review assignment logic this sprint
3. **Monthly MTTR dashboard** — build in Power BI for ops team
4. **Access Management deep-dive** — investigate root cause of high breach rate

---
*Analysis performed using Python (Pandas, Matplotlib, Seaborn)*
*Dataset: 5,000 synthetic tickets modelled on ServiceNow schema*
