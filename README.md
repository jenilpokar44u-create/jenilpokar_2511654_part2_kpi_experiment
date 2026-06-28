# Part 2: KPI Framework, Business Experiment Analysis & Decision Recommendation

## Business Context
I analyzed an A/B test dataset comparing our legacy onboarding experience (Control) against a newly designed onboarding and activation campaign (Treatment) to determine whether the new experience should be permanently rolled out to all users.

## Dataset Description
* **File:** `campaign_experiment_data.xlsx`
* **Volume:** 1,394 unique users evaluated across behavioral steps (landing page visits, trial starts, onboarding completions) and post-conversion guardrails (revenue, support tickets, refunds).

## Analytics Approach & Data Preparation
I verified the dataset for structural integrity prior to testing:
* Confirmed 0 duplicate user IDs.
* Verified binary indicators were strictly limited to `0` and `1`.
* Flagged missing fields in optional tracking attributes (`traffic_source`), which were preserved for high-level segment reviews.

## Metric Framework & KPI Tree Summary
* **North Star Metric:** Paid Conversion Rate.
* **Primary Drivers:** Top-of-Funnel Engagement, Activation & Onboarding, Monetization & Trial.
* **Guardrails Evaluated:** Refund Rate, Support Ticket Rate, and Average Engagement Score.

## Experiment & Hypothesis Test Summary
I conducted a two-proportion Z-test on the core conversion outcomes:
* **Control Conversion:** 5.1%
* **Treatment Conversion:** 8.4%
* **P-Value:** 0.019 (Statistically Significant, Null Hypothesis Rejected).

## Final Strategic Recommendation
**LAUNCH.** The performance gains are statistically validated, engagement scores are up, and our core guardrail metrics (Refunds and Support Tickets) show no signs of dangerous business risk.

## Repository Visual Elements
* KPI Tree Schematic: `outputs/kpi_tree.png`
* Data Metrics Summary: `screenshots/summary_metrics.png`
* Statistical Evidence: `screenshots/hypothesis_test_output.png`