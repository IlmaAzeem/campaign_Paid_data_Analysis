**Why We Needed This**
Managing multiple marketing campaigns across products was time-consuming and error-prone. Our team had to manually download data from Google Ads, calculate daily KPIs (CTR, CPC, CVR, CPA, ROI), and identify underperforming campaigns.
This manual process:
1)Consumed 2–3 hours daily.
2)Delayed performance detection.
3)Increased chances of missing campaign issues early (e.g., CPC spikes, drop in ROI).
To eliminate repetitive tasks and enable real-time performance visibility, we decided to automate campaign data extraction, aggregation, and alerting using the Google Ads API.

**How:**
Built a Python automation that pulls campaign-day metrics (impressions, clicks, cost, conversions, value) via Google Ads API, aggregates them to daily campaign level, and calculates KPIs — CTR, CPC, CVR, CPA, ROI.
The system compares the latest-day metrics with 30-day historical averages and flags deviations beyond set thresholds.
It exports detailed CSV/XLSX reports and sends HTML email alerts to the marketing team.

**Challenges:**
Handled API rate limits, missing values, and dynamic threshold configuration; optimized email formatting for cross-client readability.

**Outcome & Impact**
✅ Reduced daily manual monitoring time from 2–3 hours to under 5 minutes.
✅ Enabled proactive decision-making — marketing team received alerts the same day a campaign started deviating.
✅ Improved data accuracy and transparency across stakeholders.
✅ Framework now easily extendable to include other ad platforms (Meta Ads, LinkedIn Ads).

