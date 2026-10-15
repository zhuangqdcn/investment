---
name: stock-monitoring-research
description: 'Monitor recent company developments and stock price movements, update a stock watchlist, and assess short-term and long-term outlooks. Use for stock monitoring, what changed since the last report, recent price and news moves, one-to-four-week forecasts, and six-to-twelve-month scenarios with current sources.'
argument-hint: 'Companies or tickers; optional exchanges, previous report, news window, short-term horizon, long-term horizon, and as-of date'
---

# Stock Monitoring Research

Monitor one or more public companies, explain recent stock and business
developments, and produce evidence-based short-term and long-term outlooks.
Separate measured historical movements from uncertain future scenarios.

## Scope

- Run a fresh research snapshot on each invocation. This skill does not run in
  the background, schedule checks, retain state automatically, or send alerts.
  Recurring monitoring requires a separately configured scheduler and data
  access; never claim either is active without verification.
- Accept a company, ticker, or watchlist. Use tickers supplied in the request or
  an explicitly available previous watchlist; do not invent holdings. If none
  is available, request the target companies before researching.
- Default to the past seven calendar days for news, the latest trading session,
  five trading sessions, and one month for price changes, 1-4 weeks for the
  short-term outlook, and 6-12 months for the long-term outlook.
- Honor requested windows and state their exact dates. Report in the user's
  language. This is investment research, not personalized investment advice.
- Return the report in chat. Do not modify the workspace, save watchlists or
  report files, or configure automation unless explicitly requested.

## Workflow

### 1. Establish the monitoring baseline

- State the as-of date, time zone, research windows, and both forecast horizons.
  For a historical as-of request, use only information available by that date;
  exclude later filings and hindsight.
- Verify each company's legal name, ticker, exchange, currency, share class,
  and listing status using official company or exchange sources. Distinguish
  ADRs, ordinary shares, similarly named companies, and dual listings.
- Use a previous report only when actually provided or accessible with
  authorization. Record its timestamp and compare like-for-like metrics.
  Otherwise label this a first snapshot with no prior baseline.
- Keep the requested watchlist intact. If a listing cannot be resolved,
  disclose the ambiguity and omit its numerical analysis rather than silently
  substituting another security.

### 2. Refresh and verify evidence

- Use available web search, browsing, or market-data tools. Refresh sources on
  every run; do not treat model knowledge or an old report as current evidence.
- Prefer company investor relations, regulatory filings, earnings releases,
  exchange notices, and official macroeconomic releases. Use reputable news
  and market-data providers for timely context and price history.
- Search for positive and negative developments: earnings and guidance,
  demand, margins, products, contracts, financing, dilution, capital returns,
  leadership changes, lawsuits, regulation, competitors, and macro shocks.
- Start with the requested news window; expand to 30 days and the latest
  financial reports for context. Mark older events as background.
- Record event dates separately from publication dates. Corroborate material
  disputed claims and investigate corrections or recovery updates.
- Label facts, management guidance, consensus estimates, analyst opinions,
  rumors, and your own interpretations separately. Treat social-media claims
  as unverified leads, not established catalysts.
- If access fails or data is unavailable, explicitly report which source or
  metric could not be checked and how that limits the outlook. Never invent
  prices, news, dates, estimates, citations, or successful monitoring results.

### 3. Measure recent stock movements

- Report the latest verifiable price with its source timestamp, time zone,
  currency, and session (regular, premarket, or after-hours). State whether it
  is live, delayed, or an end-of-day close; if delay is unknown, say so.
- For each return window, give the actual starting and ending trading dates.
  Use comparable regular-session closes rather than mixing intraday and closing
  prices. Compute price return as `(end / start - 1) * 100`.
- Account for splits and other corporate actions using a consistent series.
  Disclose whether prices are raw, split-adjusted, or dividend-adjusted; label
  total returns separately from price returns. If adjustment is unverified,
  qualify or omit the comparison.
- Compare the stock with an appropriate broad-market and sector benchmark
  over identical dates and on the same return basis. Express stock return
  minus benchmark return in percentage points.
- Include volume relative to a stated historical average and volatility only
  when the required data is verified. Do not infer abnormal volume or calculate
  technical indicators from missing history.
- Separate observed moves from possible explanations. Timing alone does not
  prove that a news item caused a price change; consider sector and market moves.

### 4. Explain company changes and monitoring signals

- Rank material developments by likely relevance, not headline count. Explain
  the path from each event to revenue, margins, cash flow, financing risk,
  valuation, or investor expectations.
- Separate genuinely new information from old or apparently priced-in context.
  Do not equate a positive business event with a guaranteed positive return.
- When a baseline exists, mark items as new, changed, resolved, or unchanged.
  Explain what evidence changed the outlook; compare prior scenarios without
  rewriting the old prediction or implying it was more accurate than it was.
- Identify verified upcoming earnings, guidance, regulatory decisions, product
  milestones, and other catalysts. Distinguish confirmed dates from estimates.
- Give observable monitoring triggers, their sources, and why they matter.
  Prioritize major guidance changes, financing events, material filings, and
  verified unusual price/volume moves. Do not claim alerts have been delivered.

### 5. Build two independent outlooks

- **Short term, 1-4 weeks:** assess catalysts, earnings expectations, sector
  momentum, positioning when verified, volatility, and macroeconomic releases.
  Flag immediate 1-3-trading-day event or gap risk separately.
- **Long term, 6-12 months:** assess revenue and earnings trajectory, margins,
  cash generation, balance sheet, dilution, competitive position, execution,
  valuation, and sensitivity to rates and industry demand. Cite dates and
  assumptions for valuation inputs and distinguish estimates from reported data.
- Provide base, bullish, and bearish scenarios for each horizon. For each,
  state direction, catalyst or assumption, causal reasoning, confirmation
  evidence, and an observable invalidation condition.
- Explain why the horizons may disagree, such as a near-term earnings rally
  despite longer-term valuation or funding risk.
- Use qualitative direction when evidence cannot support a numeric range.
  Any return range or price target must state its verified reference price,
  horizon, method, assumptions, and supporting evidence; it is not a promise.
- Do not force unsupported scenario probabilities. If used, label them
  subjective, explain their basis, and make each horizon's probabilities sum
  to 100%. Confidence describes evidence quality, not probability of profit.
- Do not make guaranteed predictions or personalized buy/sell, leverage, or
  position-sizing recommendations.

## Report Format

Keep the summary concise; use per-company detail to support the conclusions.

1. **As-of and coverage:** timestamps, watchlist identities, windows, baseline
   status, source freshness, and missing-data limitations.
2. **Watchlist summary:**

   | Company / ticker / exchange | Latest verified price and timestamp | Last session / 5 sessions / 1 month | Benchmark-relative move | Key new development | Short-term outlook | Long-term outlook | Evidence confidence |
   | --- | --- | --- | --- | --- | --- | --- | --- |

   Use `Unavailable` with an explanation for unsupported fields, not zero or
   invented values. Specify benchmark names and comparison dates in the detail.
3. **Per-company evidence:** dated news, measured price moves, company changes,
   benchmark context, plausible explanations, and differences from the baseline.
4. **Per-company scenarios:** separate short-term and long-term tables:

   | Scenario | Direction / supported range | Drivers and assumptions | Confirmation signal | Invalidation signal |
   | --- | --- | --- | --- | --- |

5. **What to monitor next:** event or metric, confirmed or estimated date,
   observable trigger, potential impact, and source.
6. **Risks and sources:** unresolved gaps, alternative explanations, and dated
   links supporting material news, prices, filings, and calendar claims. Attach
   citations to the relevant claims rather than only giving a generic link list.

## Completion Check

- Every requested company is covered or explicitly listed as unresolved.
- Historical moves have verified dates, timestamps, currency, and return basis.
- Both horizons have distinct base, bullish, and bearish scenarios.
- Baseline changes are supported, or the report clearly says first snapshot.
- Material claims have dated sources; unavailable data is explicitly disclosed.
- Facts and forecasts are distinct, uncertainty is visible, and no autonomous
  monitoring, persistent state, delivered alerts, or guaranteed returns are
  falsely claimed.
