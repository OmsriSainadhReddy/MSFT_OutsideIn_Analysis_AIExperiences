# Consumer Copilot: where the next growth comes from

An outside-in analysis of Microsoft's consumer revenue, built only from public filings and earnings calls.

**[Open the interactive dashboard](https://omsrisainadhreddy.github.io/MSFT_OutsideIn_Analysis_AIExperiences/)** · [Read the two-page memo](memo.md) · [Excel model](msft_consumer_ai_model.xlsx)

## The question

Microsoft's two consumer revenue engines are slowing at the same time. Search ad growth (ex-TAC) fell from 21% to 10% over FY26, with mid-single digits guided next. Microsoft 365 consumer growth was lifted by the Copilot price increase: in FY26 Q2, consumer cloud revenue grew 29% while subscriptions grew 6%. That effect is now wearing off, and growth is guided down to the mid-teens.

So where should the next consumer Copilot dollar come from?

## What I found

| Option | Three-year value* | Main risk |
|---|---|---|
| Scale ads in free Copilot | $656M | How much of the revenue would have come through Bing anyway |
| Launch a low-price AI plan (~$8 a month) | $498M | Whether free users convert |
| Move more subscribers from Family to Premium | $388M | Small base; extra AI usage costs |

*Net present value of gross profit, FY27 to FY29, base case. Every assumption can be changed on the dashboard.

**Recommendation:** scale ads first, test the low-price plan in a few markets with a pass mark of about 1.2% paid conversion, and keep the Premium upsell running.

**What would change the answer:**
- Ads fall behind the Premium upsell if they earn under about $2 per user a year by FY29.
- The low-price plan only beats the Premium upsell if more than about 1.2% of free users pay for it.

Both can be measured before committing.

## A live forecast check

Before forecasting, I tested how accurate Microsoft's own search-ads guidance has been. Results beat the guidance midpoint in four of the last five quarters, by 2.2 points on average. Adjusting guidance for that pattern cut the average forecast error from 2.5 to 1.6 points.

Using that method, here is my forecast for FY27 Q1 (July to September 2026), committed before Microsoft reports in late October 2026:

| Metric | Microsoft guidance | My forecast | Actual |
|---|---|---|---|
| Search ad revenue growth, ex-TAC | 4% to 6% | 7.2% | Pending |
| Search and advertising growth, ex-TAC (restated) | 6% to 8% | 9.2% | Pending |

The forecast is tagged as release [`fy27q1-forecast`](../../releases/tag/fy27q1-forecast), so its date can be checked.

## How it's built

- **Data:** eight quarters of revenue by business line from Microsoft's September 2026 restatement filing, plus guidance wording from five earnings call transcripts. Every number in `data/` has a source URL.
- **Guidance check:** compares three forecasting methods against actual results.
- **Business case:** sizes the three options over FY27 to FY29, with sensitivity grids showing when the answer flips.
- **Assumptions:** where Microsoft doesn't disclose a number (subscriber count, AI cost to serve, ad yield, conversion), it is an assumption, listed with its reasoning in `data/assumptions.csv`.

Microsoft's fiscal year runs July to June: FY26 is July 2025 to June 2026.

## Files

```
index.html                       Interactive dashboard
memo.md                          Two-page written argument
msft_consumer_ai_model.xlsx      Same model with live formulas
data/
  quarterly_revenue.csv          Revenue by business line, FY25 Q1 to FY26 Q4
  growth_metrics.csv             Growth rates disclosed by Microsoft
  guidance_history.csv           Guidance wording, assumed range and actual
  assumptions.csv                Every assumption, its value and why
  sources.csv                    Every source with its URL
forecasts/fy27_q1.csv            FY27 Q1 forecast, committed before results
```

## Limits

Independent work using public information only. Not affiliated with or endorsed by Microsoft. Several inputs are assumptions, labelled as such, and internal data would likely change them. Built with the help of AI tools; every figure is sourced and was checked against Microsoft's filings.

---

Omsri Yarram · Pricing strategy and analytics · [LinkedIn](https://www.linkedin.com/in/omsri/)
