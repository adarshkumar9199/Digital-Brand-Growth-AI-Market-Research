# Digital Brand Growth & AI-Assisted Market Research
### A portfolio case study inspired by social media management work at Mangiee

**Prepared by:** Adarsh Kumar  
**Focus areas:** Social media analytics · Content strategy · Competitor benchmarking · AI-assisted ideation · Partnership lead prioritization  
**Tools demonstrated:** Microsoft Excel, structured CSV analysis, ChatGPT-assisted ideation

> **Data transparency:** This repository is a portfolio demonstration. All post-level metrics, competitor labels (Competitor A–E), prospect names and lead scores are synthetic illustrative data. They are not actual Mangiee account exports, verified competitor analytics, or researched sales leads. Do not present sample results as business outcomes. The project demonstrates the workflow and decision-making approach; real business conclusions require verified data.

---

## 1. Project at a glance

This project demonstrates how a social media or marketing team can move from scattered content observations to a more structured growth-planning process.

It brings together four connected activities:

1. **Content performance analysis:** compare posts using reach, impressions, engagement and link clicks.
2. **Competitor benchmarking:** compare content formats and engagement patterns across a sample of brands.
3. **AI-assisted content planning:** generate and organize 15 campaign concepts against objectives and measurable KPIs.
4. **Partnership lead prioritization:** use a weighted score to decide which potential brands deserve research and outreach first.

The intended outcome is not an automated marketing system. It is a practical decision-support workflow that helps a marketer ask better questions, identify experiments, and prioritize the next action.

## 2. Business context and problem statement

A brand may publish regularly but still struggle to answer questions such as:

- Which content formats appear to attract more attention?
- Which posts encourage meaningful interaction rather than only passive views?
- Are we measuring awareness, engagement and traffic separately?
- What can we learn from competitor content without blindly copying it?
- How can a small team maintain a consistent pipeline of relevant content ideas?
- Which potential partner brands should be researched first?

Without a consistent framework, teams may rely on likes alone, compare brands with different audience sizes, or create content without a clear objective.

**Project objective:** create a simple, repeatable framework that connects content metrics, competitor observations, campaign ideas and outreach priorities.

## 3. Scope and deliverables

| Workstream | What was created | How a marketer could use it |
|---|---|---|
| Social media analysis | Sample post-level dataset and performance analysis notes | Compare content and identify formats/themes to test |
| Competitor benchmarking | Brand-level comparison table for six labels | Review reach, engagement and link-click patterns together |
| Campaign ideation | 15 structured content concepts | Build an awareness, education, trust and consideration calendar |
| Lead prioritization | Weighted scoring model and sample prospect sheet | Rank prospects for further research and personalized outreach |
| Documentation | Data dictionary, methodology and interview guide | Explain assumptions, formulas, limitations and next steps |

## 4. Dataset overview

The repository includes **60 illustrative Instagram post records**: 10 records for Mangiee and 10 for each of five anonymized competitor labels.

The post-level file includes:
- Post identifier, brand label, platform and date
- Content format and theme
- Followers at the time of the sample post
- Reach and impressions
- Likes, comments, shares and saves
- Link clicks
- Total engagements, engagement rate and impressions per reached user

Other datasets:
- `competitor_analysis.csv`: one summary row per brand label.
- `brand_lead_scoring.csv`: 10 fictional prospects with three assessment scores and a weighted priority.
- `campaign_ideas.csv`: 15 content concepts with format, direction, objective and success metrics.

**Important:** the dates and values are constructed sample observations. The six brand labels are not a verified competitive set. The sample is useful for demonstrating calculations and dashboard design, not for claiming market truth.

## 5. Analytical workflow

### Step 1 — Define the question before looking at the numbers

The analysis is organized around practical marketing questions:
- Distribution: how many unique accounts did the content reach?
- Visibility: how many impressions were generated?
- Interaction: how many likes, comments, shares and saves were recorded?
- Traffic: how many link clicks were recorded?
- Efficiency: how much interaction occurred relative to reach?

### Step 2 — Calculate engagement consistently

For this project, total engagements are defined as:

`Engagements = Likes + Comments + Shares + Saves`

The sample engagement-rate formula is:

`Engagement Rate (%) = (Engagements / Reach) × 100`

Reach is used as the denominator because this version is designed to measure interactions relative to accounts reached. Some platforms or teams use followers or impressions as the denominator; comparisons are meaningful only when the definition is consistent and clearly stated.

### Step 3 — Compare multiple metrics, not one vanity metric

- **Reach** helps assess distribution.
- **Impressions** represent total displays and may include repeat views.
- **Engagement rate** helps assess interaction relative to reach.
- **Shares and saves** can indicate that content is useful or worth revisiting.
- **Link clicks** are a stronger signal of traffic intent than likes alone, but do not prove a sale or conversion.

A high reach figure does not automatically mean a post was successful. The right metric depends on the campaign objective.

### Step 4 — Segment and interpret

The analysis notes recommend looking at performance by content format and theme. For example, Reels, carousels, static posts and Stories serve different purposes. A fair comparison should account for audience size, posting period, paid versus organic distribution, creative quality and campaign objective.

### Step 5 — Convert observations into experiments

The campaign idea sheet turns broad observations into testable content concepts. Each idea includes:
- Format and creative direction
- Intended objective (awareness, consideration, trust, education, engagement or conversion support)
- Suggested success metrics

The next step would be to publish controlled tests, compare results against a baseline, and retain or revise ideas based on verified performance.

## 6. Competitor benchmarking approach

Mangiee and five anonymized competitor placeholders are compared across:
- Average reach
- Average impressions
- Average engagement rate
- Average link clicks
- Most frequently observed content type in the sample

**How to interpret it:** compare engagement rate alongside reach. A smaller account can have a higher engagement rate while a larger account generates more total reach or clicks. Neither metric alone establishes which brand has the better strategy.

The sample competitor labels must be replaced with a clearly defined and verified competitor set before this can be used as actual market research. Record each public post URL, date observed, platform, format and the date range used. Keep paid and organic content separate wherever possible.

## 7. AI-assisted campaign ideation

The project includes 15 ideas across Reels, carousels, static posts and Stories. They are grouped around practical content purposes:

- **Awareness:** short problem-solver videos and relevant trend adaptations.
- **Education:** myth-versus-fact posts, checklists and beginner guides.
- **Trust:** behind-the-scenes content and permission-based customer stories.
- **Engagement and research:** polls, Q&A and audience preference questions.
- **Consideration:** product demonstrations, use cases and transparent comparisons.
- **Community:** approved user-generated content and monthly roundups.

AI is used as an ideation assistant, not as an authority. A human marketer must check product claims, brand voice, originality, permissions, competitor references and platform policies before publishing.

## 8. Partnership lead prioritization model

The sample model scores each prospect from 1 (low) to 5 (high) on three factors:

| Factor | Weight | What it means |
|---|---:|---|
| Branding needs | 35% | Potential gaps in positioning, visual consistency, storytelling or content |
| Online presence | 30% | Website/social activity, consistency and discoverability |
| Growth signals | 35% | Public signals such as launches, expansion, hiring or campaign activity |

**Weighted score:**

`(Branding Needs / 5 × 35) + (Online Presence / 5 × 30) + (Growth Signals / 5 × 35)`

Suggested bands:
- High priority: 75–100
- Medium priority: 60–74.9
- Low priority: below 60

The score is a triage aid, not a prediction of conversion or revenue. Before contacting a real business, record evidence, source links and the date checked. A high score should lead to further research and personalized outreach, not an automatic sales claim.

## 9. Recommended dashboard layout

If presenting the Excel dashboard, organize it so a reviewer can move from an overall view to a specific question:

**Top-level KPI cards**
- Total posts in the selected sample
- Average reach
- Average impressions
- Average engagement rate
- Average link clicks

**Suggested visuals**
1. Average engagement rate by brand
2. Average reach and impressions by brand
3. Engagement by content format
4. Link clicks by brand or content format
5. Lead-priority distribution (High / Medium / Low)

**Useful filters**
- Brand
- Content format
- Content theme
- Date or period

Use consistent metric definitions, clear units, descriptive chart titles and filters that do not mix incomparable records. Do not label sample data as live analytics.

## 10. Key interpretation framework

| Pattern | Possible interpretation | What to test next |
|---|---|---|
| High reach + high engagement rate | Content may be both distributed and relevant | Repeat the format with a new angle |
| High reach + low engagement rate | Distribution is strong, interaction is weaker | Review hook, audience fit and CTA |
| Low reach + high engagement rate | Reached audience may find it relevant | Improve distribution and discoverability |
| Low reach + low engagement rate | Both distribution and interaction need review | Revisit creative, topic, timing and audience |

These are diagnostic prompts, not guaranteed causal explanations. One post is not enough to establish a trend.

## 11. Limitations and responsible use

- All numerical records and placeholder labels are synthetic.
- The sample has only 10 posts per brand, which is too small for strong generalizations.
- The dataset does not include verified paid/organic status, campaign spend, audience demographics, conversion events or sales.
- Reach and impressions can be affected by platform algorithms, timing, account size and paid promotion.
- The lead scores are subjective illustrative inputs, not validated predictors.
- AI-generated ideas require human review and brand-specific adaptation.
- No real business uplift, follower growth, revenue increase or campaign result is claimed.

## 12. Future improvements

1. Replace sample records with authorized platform exports or carefully documented public observations.
2. Use a consistent 30–90 day observation window and capture source URLs/post IDs.
3. Separate organic and paid posts; add campaign objective and spend where available.
4. Add audience segments, CTA type, video watch time and conversion events.
5. Calculate format-level averages and distributions using a larger sample.
6. Add a before/after experiment log and define a baseline before each campaign.
7. Validate lead-scoring weights against actual outreach outcomes.
8. Add a documented Excel workbook with refreshable tables, formulas, slicers and dashboard screenshots.

## 13. Repository structure

```text
.
├── README.md
├── PROJECT_NOTES.md
├── data/
│   ├── README.md
│   ├── social_media_posts.csv
│   ├── competitor_analysis.csv
│   └── brand_lead_scoring.csv
├── analysis/
│   ├── content_performance.md
│   ├── competitor_benchmarking.md
│   └── brand_prioritization.md
├── ai_content/
│   ├── campaign_ideas.md
│   └── campaign_ideas.csv
└── docs/
    ├── INTERVIEW_PREP.md
    ├── METRICS_AND_METHODOLOGY.md
    └── CONTENT_STRATEGY_PLAYBOOK.md
```

## 14. How to explore the project

1. Start with this README for the overall business context.
2. Read `data/README.md` before interpreting any CSV.
3. Open `data/social_media_posts.csv` to inspect the sample post-level records.
4. Read the three files in `analysis/` for the analytical logic.
5. Open `ai_content/campaign_ideas.csv` to review the 15 content concepts.
6. Read `docs/INTERVIEW_PREP.md` to understand how to explain the project and answer follow-up questions.

The CSV files can be opened in Microsoft Excel or Google Sheets. This repository currently documents the data and analytical workflow; do not assume a live dashboard or live data connection unless the corresponding workbook is present and verified.

## 15. Author

**Adarsh Kumar**  
GitHub: [@adarshkumar9199](https://github.com/adarshkumar9199)

---

*This is a learning and portfolio case study. Replace illustrative data with verified evidence before making real-world marketing, competitor or sales decisions.*
