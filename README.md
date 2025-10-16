Pulls campaign×day metrics (impressions, clicks, cost, conversions, conversion value) from Google Ads API.
Aggregates to daily campaign-level metrics and computes derived metrics: CTR, CPC, CVR (conversion_rate), CPA, ROI.
Computes historical averages (configurable window, default 30 days) per campaign and flags breaches when latest-day metrics deviate beyond percent-change thresholds you configure.
Exports:
daily_all_YYYYMMDD.csv — all campaign-days
daily_target_YYYYMMDD.csv — campaigns on the target/latest date
alerts_YYYYMMDD.csv — alerts (breaches)
campaign_report_YYYYMMDD.xlsx — workbook with those sheets
Sends an HTML email to the marketing recipient(s) with the alert table (if any). If SMTP env vars are missing, it still exports the reports and prints a notice.
