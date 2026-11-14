# CULT+MATH open data

Tables behind CULT+MATH research studies, published as CSV under CC BY 4.0.
Each folder matches one study on cultmath.com. Read the study page for the
method, the controls and what the numbers do and do not show.

Ipalibo Da-Wariboko · CULT+MATH LLC · November 14, 2026

## Studies

| Folder | Study | Source | Files |
|---|---|---|---|
| `advertising-intensity/` | [Advertising intensity across US public filers, CY2024](https://cultmath.com/research/marketing/advertising-intensity) | SEC XBRL (data.sec.gov) | categories, named filers, rejected rows |
| `cpg-margin-recovery/` | [Gross margin in US food and household filers, FY2019 to latest](https://cultmath.com/research/cpg/margin-recovery) | SEC XBRL company facts | filers, SIC groups, controls |
| `semiconductor-margins/` | [Semiconductor and hardware gross margin, FY2019 to latest](https://cultmath.com/research/semiconductors/sourcing-concentration) | SEC XBRL company facts | semiconductor filers, hardware filers, excluded filers, rejected tags |

Rejected and excluded rows are published on purpose. They show what the
validation removed and why.

## Column notes

- `*_pct` columns are percentages (33.55 means 33.55%).
- `change_pts` is percentage points, latest fiscal year minus FY2019.
- Gross margin is (revenue − cost of goods) ÷ revenue, with candidate revenue
  tags tested against cost of goods. `revenue_tag` names the tag used.
- `cv` is the coefficient of variation inside a category (stdev ÷ mean).

## What is not here, and why

Only tables whose sources are all public domain or freely redistributable are
in this repo. Left out:

| Left out | Why |
|---|---|
| Import unit values and partner shares (margin-recovery, sourcing-concentration) | UN Comtrade terms of use are not clear enough for redistribution |
| Search volume studies (Netflix engagement, demand decay, spinoff halo and others) | Google Ads volumes via DataForSEO; vendor terms do not allow redistribution |
| AI answer studies (who answers dinner, retrieval signature, unbuyable share, vendor disagreement) | Captured assistant answers; terms unclear |
| TV audience, YouTube and review studies | Third-party measurement and platform data |

The study pages still show these findings. Only the raw tables stay off GitHub.

## Use it from an AI assistant

CULT+MATH runs an MCP server that searches and returns the full studies.
See `mcp/README.md` or [cultmath.com/agent](https://cultmath.com/agent).

## License and citation

Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit
CULT+MATH and link the study page. Suggested citation:

> Da-Wariboko, I. (2026). *[Study title]*. CULT+MATH. https://cultmath.com/research/…

The underlying SEC filings are public domain. CULT+MATH's selection,
validation and derived figures are what the license covers.

## Related

- Research index: https://cultmath.com/research
- Frameworks: https://cultmath.com/frameworks
- Sound Decisions: https://cultmath.com/blog
