# Consumer Copilot: where the next growth comes from

**An outside-in view, built from public filings. October 2026.**
Prepared by Omsri Yarram. Model: `model/msft_consumer_ai_model.xlsx`; data: `data/`.

*Microsoft's fiscal year runs July to June. FY26 is July 2025 to June 2026; FY27 Q1 is July to September 2026.*

## Summary

Both of Microsoft's consumer revenue engines are slowing at the same time. Microsoft 365 consumer revenue grew about 24% in FY26, largely as the Copilot price increase reached renewing customers, and Microsoft now guides consumer cloud growth to the mid-teens. Search ad growth (ex-TAC) fell from 21% to 10% over the same year, with mid-single digits guided for FY27 Q1.

I sized three ways to restore growth from consumer Copilot. On my assumptions, leaning harder on ads in free Copilot has the highest value. A low-price AI tier comes second, but only if it converts more than about 1.2% of free users. Pushing more subscribers to Premium is the smallest but safest. My suggestion is to scale ads first, run the low-price tier as a test with that conversion gate, and keep the Premium push running in the background.

## The setup

| | FY25 Q4<br>Apr–Jun 2025 | FY26 Q1<br>Jul–Sep 2025 | FY26 Q2<br>Oct–Dec 2025 | FY26 Q3<br>Jan–Mar 2026 | FY26 Q4<br>Apr–Jun 2026 | FY27 Q1 guide<br>Jul–Sep 2026 |
|---|---|---|---|---|---|---|
| Search ad revenue ex-TAC growth | 21% | 16% | 10% | 12% | 10% | Mid-single digits |
| M365 consumer products and cloud growth | | 28% | 27% | 26% | 16% | Mid-teens (cloud) |

Two things stand out. First, consumer growth came mostly from price: in FY26 Q2, consumer cloud revenue grew 29% while subscriptions grew 6%. That price effect is now lapping. Second, the new Devices and Consumer segment is guided to about $14.95B at the midpoint for FY27 Q1, roughly 7% below a year ago, with Windows OEM and XBOX declining. Advertising is the only growing line left in that segment.

Microsoft no longer discloses consumer subscriber counts, so I derived about 87M paid subscribers from revenue and an assumed blended price. That number drives Option A and should be checked against internal data first.

## Three options, sized over FY27 to FY29

Gross profit NPV at a 9% discount rate. Each option is incremental to the current plan and sized on its own.

| Option | FY29 revenue | FY29 gross profit | 3-year NPV | Where it lands |
|---|---|---|---|---|
| A. Move more subscribers from Family to Premium | $349M | $243M | $388M | M365 consumer cloud |
| B. Launch a $7.99 AI tier without Office apps | $569M | $342M | $498M | M365 consumer cloud |
| C. Scale ads in free Copilot | $503M | $428M | $656M | Search and advertising |

**A. Premium upsell.** Premium share rises from an assumed 4% to 10% of subscribers by FY29, at a $70 annual step from Family. Low risk, since the product and price already exist. It is limited by the size of the base and by the extra AI cost of heavier users.

**B. Low-price AI tier.** Priced against Google AI Plus ($7.99) and ChatGPT Go ($8), aimed at the free Copilot audience that does not need Office apps. It brings in the most revenue but carries serving and acquisition costs. The base case assumes conversion of free monthly users rising to 1.5% by FY29.

**C. Scale ads in free Copilot.** Microsoft already serves ads in Copilot. This option assumes ad revenue per user in ad markets reaches $3 a year by FY29, about 20% of what Bing earns per user today, and that 30% of it replaces Bing revenue that would have happened anyway. It has the highest margin because it uses the existing ad stack and serves users Microsoft is already paying to serve.

## When the answer changes

The ranking depends on two numbers, and both can be tested before committing.

- **Option C beats Option A as long as ad revenue per user reaches about $2 by FY29 and Bing cannibalisation stays under roughly 35 to 40%.** At $3 per user, C beats A even if half its revenue comes out of Bing. At $1 per user, it never does.
- **Option B beats Option A only if FY29 conversion exceeds about 1.2% at $7.99.** For context, ChatGPT converts roughly 5% of its weekly users to paid, but Copilot's free audience is largely reached through Windows and Edge by default, so it may convert well below that.

## Suggested next steps

1. **Measure cannibalisation directly.** Hold out a group of Copilot users from ads and compare their Bing usage and ad revenue against users who see ads. This settles the main risk in Option C.
2. **Test the low-price tier in one or two markets** with a pre-set go/no-go threshold: at least 1.2% conversion of active free users by month six, with downgrades from Personal tracked separately.
3. **Keep the Premium push running** through in-app prompts when Family owners hit Copilot usage limits.

## Risks this analysis does not capture

- Ads could make free users less willing to pay, slowing Options A and B. ChatGPT's choice to show ads only on its Free and Go tiers suggests ads and upgrades can coexist, but that is one data point.
- Costs to serve AI use are assumptions; Microsoft does not disclose them.
- Regulators in several countries have already questioned how the Copilot price increase was communicated. A new tier or more ads would face the same scrutiny.

## Appendix: forecasting method and a live test

The model includes a backtest of Microsoft's own guidance for search ads across five quarters (FY25 Q4 to FY26 Q4). The actual result came in above the guidance midpoint in four of the five, by 2.2 points on average. The exception was FY26 Q2, which Microsoft described as slightly below expectations due to execution challenges. Adding the average past beat to the guidance midpoint cut the average error from 2.5 points to 1.6 points across the four quarters where it could be applied; simply carrying forward last quarter's growth did worse than either over the same quarters, at 3.8 points. Five quarters is a small sample, so this is a pattern to watch rather than a rule.

Applying the same method to FY27 Q1 (July to September 2026), before Microsoft reports in late October 2026:

| | Guidance | My forecast |
|---|---|---|
| Search ad revenue ex-TAC growth (as-reported basis) | 4% to 6% | about 7.2% |
| Search and advertising ex-TAC growth (restated basis) | 6% to 8% | about 9.2% |
| Search advertising revenue (reported) | | about $3.87B |
| M365 consumer products and cloud revenue | Mid-teens growth (cloud) | about $2.53B |

## Sources and limits

Revenue by business line comes from Microsoft's September 2026 restatement filing (Form 8-K, Exhibit 99.1) and FY26 earnings releases. Guidance wording comes from earnings call coverage. Consumer prices and competitor figures come from published price pages and third-party reports, listed in the model's Sources tab. Every assumption is marked in blue in the model and can be changed. This is independent work using public information only, and internal data would likely move several of these numbers.
