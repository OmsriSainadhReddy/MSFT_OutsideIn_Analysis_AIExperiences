# Consumer Copilot: where the next growth comes from

An outside-in analysis of Microsoft's consumer revenue, built only from public filings and earnings calls: a backtest of Microsoft's own guidance, a live FY27 Q1 forecast, and a business case for three ways to grow consumer Copilot revenue.

**Live dashboard:** `https://<your-github-username>.github.io/<repo-name>/`

Microsoft's fiscal year runs July to June: FY26 is July 2025 to June 2026, and FY27 Q1 is July to September 2026.

## Files

```
index.html                  Dashboard (GitHub Pages serves this)
memo.md                     Two-page written argument
model/
  msft_consumer_ai_model.xlsx   Same model with live formulas
data/
  quarterly_revenue.csv     Revenue by business line, FY25 Q1 to FY26 Q4
  growth_metrics.csv        Growth rates disclosed by Microsoft
  guidance_history.csv      Guidance wording, assumed range and actual, by quarter
  assumptions.csv           Every assumption, its value and why
  sources.csv               Every source with its URL
forecasts/
  fy27_q1.csv               FY27 Q1 forecast, published before results
```

Every number in `data/` has a source URL, so it can be checked against Microsoft's filings and earnings calls.

## Headline results (base case)

- Search ad growth (ex-TAC) fell from 21% to 10% over FY26; Microsoft 365 consumer growth is guided down to the mid-teens.
- Microsoft's search ad results beat the guidance midpoint in four of the last five quarters, by 2.2 points on average. Adjusting guidance for that pattern cut forecast error from 2.5 to 1.6 points.
- Three-year gross profit value: scaling ads in free Copilot $656M, a low-price AI plan $498M, a Premium upsell $388M.
- The low-price plan only beats the Premium upsell if it converts more than about 1.2% of free users.

## Publish on GitHub Pages

1. Create a public repo and upload the files in the layout above.
2. Settings, then Pages: deploy from the `main` branch, root folder.
3. In `index.html`, set `CONTACT_URL` to your LinkedIn URL. After Microsoft reports FY27 Q1, set `FY27Q1_ACTUAL` (for example `0.07`) and fill the `actual` column in `forecasts/fy27_q1.csv`.

## Limits

Independent work using public information only. Not affiliated with or endorsed by Microsoft. Subscriber counts, cost to serve, ad yield and conversion are assumptions, labelled as such, and internal data would likely change them.
