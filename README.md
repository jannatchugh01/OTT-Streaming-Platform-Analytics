# Lio–Jotstar OTT Analytics | Power BI

A Power BI project analysing two streaming platforms, **LioCinema** and **Jotstar**, ahead of a proposed merger. Using subscriber, content, engagement and subscription data from **January to November 2024**, I looked at where the combined platform is strong, where it is leaking users, and what to fix first.

> Lio, LioCinema and Jotstar are fictional. The scenario comes from the Codebasics Resume Project Challenge.

![Dashboard preview](https://github.com/jannatchugh01/jannatchugh01.github.io/blob/main/images/OTT.png)

---

## The Business Problem

Lio, a telecom provider, plans to merge with Jotstar, an OTT platform. Before the deal, management wanted answers to a few practical questions:

- How are subscribers growing on each platform?
- Which platform keeps its users more engaged?
- What content is actually being watched?
- Who is going inactive, and why might that be?
- How do users move between subscription plans?

## Headline Findings

| Metric | LioCinema | Jotstar |
|---|---|---|
| Total users | 183.45K | 44.62K |
| Active rate | 55.1% | 85.1% |
| Inactive users | 82.31K (44.9%) | 6.65K (14.9%) |
| Paid users | 78.45K (42.8%) | 33K (72.9%) |
| Avg. watch time per user | 25.61 hrs | 117.24 hrs |
| Total watch time | 11.03M hrs | 15.69M hrs |
| Content library | 1.25K titles | 2.36K titles |
| Users who changed plan | 13.64% | 15.89% |

**1. LioCinema has the reach, Jotstar has the engagement.**
LioCinema accounts for about 80% of combined users, yet Jotstar's much smaller base generates more total watch time (15.69M vs 11.03M hrs). Jotstar users watch roughly 4.6x more per head.

**2. Inactivity on LioCinema is a free-plan problem.**
57% of LioCinema's free users are inactive, against 33.8% on Basic and 17.9% on Premium. Free users also make up the largest share of its base (105K of 183K). Jotstar's inactivity is much lower across the board, from 6.7% on Premium to 25.7% on Free.

**3. LioCinema loses far more users to downgrades than it gains from upgrades.**
About 20.86K users downgraded against 4.16K who upgraded. The biggest flows were Basic to Free (10.3K) and Premium to Free (7.4K). Jotstar tells the opposite story: upgrades (4.35K) outnumber downgrades (about 2.7K), led by VIP to Premium (2.8K).

**4. The two platforms reach different audiences.**
LioCinema is concentrated in Tier 3 cities (79K users) and the 18-24 age group (80K). Jotstar leans towards Tier 1 (25K) and the 25-34 group (20K). Engagement follows the same pattern, with Tier 1 and younger users watching the most on both platforms.

**5. Mobile drives viewing.**
Jotstar users average 176 hrs on mobile versus 95 on TV and 81 on laptop. LioCinema shows the same ordering at a much lower level (46, 13 and 8 hrs).

**6. Growth patterns differ.**
Jotstar adds a steady ~4K users every month. LioCinema's acquisition is spiky, peaking at 37K in February and 29K in September, with some months as low as 7K, which suggests campaign-driven rather than organic growth.

**7. The content mix differs.**
Jotstar's library is half movies (50%), 35% series and 15% sports. LioCinema is 72% movies, 24% series and only 4% sports. Jotstar's top genres are Action, Drama and Thriller, with Live Matches fourth. LioCinema's lead with Drama, then Comedy and Action.

## What I'd Recommend

- **Treat LioCinema's free tier as a retention priority.** More than half of these users are inactive. Onboarding nudges, personalised recommendations and a clearer reason to stay would matter more than another acquisition push.
- **Investigate the downgrade flow.** Over 17K users dropped to Free from Basic or Premium. Pricing, content gaps and plan benefits should be reviewed before the plans are merged.
- **Use Jotstar's engagement playbook.** Its higher watch time sits alongside a large sports and series library, which LioCinema lacks.
- **Make mobile the primary experience** on the combined platform.
- **Smooth out acquisition.** Replace one-off spikes with steadier, targeted campaigns by city tier and age group.

## Analysis Structure

1. **Subscriber analysis**: growth by month, plan mix, city tier and age group, active vs inactive, paid vs free
2. **Content consumption**: watch time by age, tier, device, plan and month
3. **Content library**: titles by type, genre and language, with runtimes
4. **Upgrades and downgrades**: monthly trends and plan-to-plan transitions

Every page has slicers for age group, month and city tier.

## Tools

- **Power BI Desktop**: data modelling, DAX measures (active rate, paid rate, plan change %, watch time averages), dashboard design
- **Excel**: initial data preparation and checks
- **GitHub**: project documentation

## Repository Contents

```text
OTT-Streaming-Platform-Analytics/
├── OTT analysis.pbix                    # Power BI report
├── OTT analysis.pdf                     # Exported dashboard
├── Metrics & Analysis.pdf
├── primary_and_secondary_questions.pdf
├── problem_statement.pdf
├── meta_data.txt
└── README.md
```

## What I Took From This Project

This was good practice in turning dashboards into a business argument rather than a set of charts. The most useful part was comparing two very different platforms on the same metrics and finding that size and engagement told opposite stories.

---

**Jannat Chugh**
B.Tech ECE-AI | Data Analytics & Data Science
[GitHub](https://github.com/jannatchugh01) • [Portfolio](https://jannatchugh01.github.io/)
