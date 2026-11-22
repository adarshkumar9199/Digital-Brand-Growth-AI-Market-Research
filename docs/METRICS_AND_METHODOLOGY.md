# Metrics, Data Dictionary and Methodology

## 1. Data files

### social_media_posts.csv

One row represents one illustrative Instagram post.

| Column | Meaning |
|---|---|
| post_id | Sample post identifier |
| brand | Mangiee or anonymized competitor placeholder |
| platform | Social platform label |
| post_date | Sample observation date |
| content_type | Reel, Carousel, Static Post or Story |
| content_theme | Main theme of the post |
| followers_at_post | Illustrative follower count at post time |
| reach | Illustrative unique accounts reached |
| impressions | Illustrative total displays |
| likes | Illustrative likes |
| comments | Illustrative comments |
| shares | Illustrative shares |
| saves | Illustrative saves |
| link_clicks | Illustrative link clicks |
| engagements | Sum of likes, comments, shares and saves |
| engagement_rate_pct | Engagements divided by reach, multiplied by 100 |
| impressions_per_reached_user | Impressions divided by reach |

### competitor_analysis.csv

One row per brand label, summarizing 10 sample posts:
- posts_analyzed
- avg_reach
- avg_impressions
- avg_engagement_rate_pct
- avg_link_clicks
- top_content_type
- total_engagements

### brand_lead_scoring.csv

One row per fictional prospect:
- prospect_name: fictional placeholder
- category: illustrative business category
- branding_need_score_1_to_5: subjective assessment input
- online_presence_score_1_to_5: subjective assessment input
- growth_signal_score_1_to_5: subjective assessment input
- weighted_lead_score_0_to_100: weighted score
- outreach_priority: High, Medium or Low
- scoring_note: reminder to validate with research

### campaign_ideas.csv

One row per campaign concept:
- concept_no: idea identifier
- format: recommended content format
- campaign_concept: short concept name
- creative_direction: suggested execution
- objective: intended marketing objective
- success_metrics: suggested KPIs

## 2. Metric definitions

**Engagements** = Likes + Comments + Shares + Saves

**Engagement rate (%)** = (Engagements / Reach) × 100

**Impressions per reached user** = Impressions / Reach

**Weighted lead score** = (Branding needs / 5 × 35) + (Online presence / 5 × 30) + (Growth signals / 5 × 35)

## 3. Why multiple KPIs matter

| Objective | Primary KPIs | Supporting KPIs |
|---|---|---|
| Awareness | Reach, impressions | Frequency, video views |
| Engagement | Engagement rate, comments | Shares, saves, replies |
| Education / value | Saves, shares | Carousel completion, watch time |
| Traffic | Link clicks, CTR | Landing-page sessions |
| Lead generation | Leads, conversion rate | Form completion, cost per lead |
| Sales | Purchases, revenue, ROAS | Add-to-cart, checkout conversion |

The sample CSV does not contain all metrics in this table. These are examples of what a real campaign measurement plan could include.

## 4. Data quality checks for real data

Before analyzing actual exports:
1. Confirm the date range and timezone.
2. Remove duplicate post IDs.
3. Check missing values and zero denominators.
4. Confirm metric definitions match across platforms.
5. Separate organic and paid distribution.
6. Flag boosted posts and campaign-specific content.
7. Confirm whether link clicks mean outbound clicks, profile link taps or another event.
8. Avoid comparing different formats or objectives without context.
9. Record the export date and source.
10. Keep a copy of the untouched source export.

## 5. Interpretation cautions

- Reach is not the same as impressions.
- Engagement rate is not a sales conversion rate.
- Link clicks do not prove purchases.
- Correlation between a format and high engagement does not prove the format caused it.
- A small sample can be distorted by one unusually strong post.
- Competitor public metrics may not expose saves, reach or impressions; never invent unavailable values.
- Lead scores are prioritization aids and need evidence plus outcome validation.

## 6. Synthetic-data notice

All values currently in this repository are illustrative. They should be replaced with authorized analytics or documented public observations before being used for a real client recommendation.
