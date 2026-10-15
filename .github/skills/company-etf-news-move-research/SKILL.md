---
name: company-etf-news-move-research
description: 'Research recent news for a given public company, stock, or ETF and assess its possible price moves. Use for ticker news checks, catalyst analysis, earnings reactions, ETF outlooks, bullish and bearish scenarios, and evidence-based market-move forecasts with current sources.'
argument-hint: 'Company, stock ticker, or ETF; optional horizon, market, and as-of date'
---

# Company or ETF News and Move Research

Produce a current, source-backed briefing for a specified public company,
stock, or exchange-traded fund (ETF), then assess plausible price directions
and catalysts. Present scenarios and probabilities as uncertain research, not
as guarantees or personalized investment advice.

## Scope

- Require an identifiable company, ticker, or ETF from the request. Resolve an
  ambiguous symbol by checking the company or fund name, exchange, and region.
- Use the requested as-of date, or the current date if none is provided. State
  the date, time zone, security name, ticker, exchange, and analysis horizon.
- Default to a one-to-four-week outlook. Also note immediate event risk over
  the next one to three trading days when material.
- Research fresh information on every invocation. Do not reuse prior news,
  prices, holdings, financial figures, analyst estimates, or forecasts without
  verifying them again.
- Do not create files, modify the workspace, place trades, or commit unless the
  user explicitly asks.

## Workflow

### 1. Identify and verify the security

1. Confirm the legal company or fund name, ticker, primary exchange, currency,
   and security type using the issuer, fund sponsor, or exchange.
2. For companies, identify the industry, reporting calendar, and the main
   business drivers relevant to the requested horizon.
3. For ETFs, verify the index or active mandate, leverage or inverse exposure,
   expense ratio, assets or liquidity when relevant, top holdings, sector and
   country concentrations, and rebalance method or date.
4. Distinguish an ETF from an exchange-traded note, closed-end fund, mutual
   fund, ADR, option, or similarly named security.

### 2. Gather recent information

1. Use web search and page-reading tools to collect developments published in
   the past seven days. Expand to 30 days for context and to the latest
   earnings, filing, or fund report when necessary.
2. Check primary sources first:
   - company or fund-sponsor newsrooms and investor-relations pages;
   - regulatory filings, earnings releases, presentations, and call materials;
   - exchange notices, index-provider notices, and official macro releases.
3. Use reputable financial reporting for independent context. Treat social
   media, forums, newsletters, and unsourced aggregators only as sentiment or
   leads, never as confirmation.
4. Search for both positive and negative evidence. Include earnings, guidance,
   products, contracts, financing, capital returns, management changes,
   litigation, regulation, analyst actions, industry data, macro releases, and
   geopolitical developments when relevant.
5. For ETFs, also check material news about top holdings, sector or country
   exposures, rates, currencies, commodities, flows, distributions, index
   changes, and leverage decay or path dependency where applicable.
6. Record both publication dates and event dates. Do not cite information
   published after a historical as-of date or describe old news as new.

### 3. Validate and classify each catalyst

- Open the original source for every material claim. Search summaries and
  generated answers are discovery aids, not evidence.
- Prefer two independent sources for market-moving claims when a primary source
  is unavailable. State conflicts and unresolved gaps.
- Classify each item as confirmed fact, company or sponsor guidance, consensus
  estimate, analyst opinion, market rumor, or interpretation.
- Separate genuinely new information from already-known information. Explain
  why the market may or may not have priced it in.
- Identify the direct exposure path. For an ETF, estimate whether affected
  holdings and exposures are large enough to matter rather than assuming news
  about one constituent will move the whole fund.
- Do not invent news, quotes, URLs, dates, prices, analyst targets, consensus
  figures, holdings, or probabilities. If current evidence cannot be verified,
  say so and narrow the conclusion.

### 4. Establish market context

- If price data is available, verify the timestamp, currency, delay status, and
  source. Report the latest available price and recent returns only when
  verified; never imply access to live data.
- Compare the security's reaction with an appropriate benchmark and its sector
  or asset class. Note unusual price, volume, volatility, options activity, or
  fund flows only when supported by reliable data.
- Identify scheduled catalysts during the horizon, including earnings,
  investor days, product events, regulatory decisions, economic releases,
  distributions, index rebalances, and known lockups or financing events.
- Use valuation, technical levels, options-implied moves, short interest, and
  analyst estimates only when current, sourced, and clearly labeled. None is a
  standalone prediction.

### 5. Build move scenarios

Create a base, bullish, and bearish scenario. For each:

1. State the triggering evidence or event.
2. Explain the causal path from the catalyst to revenue, earnings, valuation,
   rates, flows, holdings, sentiment, or supply and demand.
3. Give a direction: up, down, or range-bound.
4. Give a move range only when anchored to verifiable evidence such as recent
   volatility, prior comparable reactions, options-implied movement, or
   sensitivity to underlying assets. Otherwise use qualitative magnitude.
5. Assign each scenario a rounded probability estimate, optionally with an
   uncertainty range, and make the three estimates total 100%. Explain the
   evidence behind the ranking rather than implying statistical precision.
6. List the observable signals that would confirm or invalidate the scenario.

Do not write that a move "will" happen. A catalyst can produce the opposite
price response when it is priced in, expectations differ, positioning unwinds,
or the broader market dominates.

### 6. Present the report

Use this structure:

1. **Identity and as-of time:** name, ticker, exchange, security type, horizon,
   and data freshness.
2. **Bottom line:** two to four sentences on the directional bias, confidence,
   strongest catalyst, and largest risk.
3. **Recent verified news:** date, development, classification, expected
   positive/negative/mixed effect, time horizon, and source.
4. **Security-specific drivers:** company fundamentals and event calendar, or
   ETF mandate, top exposures, concentration, and relevant constituent news.
5. **Market context:** benchmark comparison and verified price, volatility,
   flow, valuation, or positioning evidence when available.
6. **Scenario table:** scenario, probability range, direction or move range,
   triggers, and invalidation signals.
7. **What to watch next:** dated events and measurable indicators.
8. **Risks and limitations:** missing data, source conflicts, pricing status,
   and factors that could overwhelm the thesis.
9. **Sources:** clickable primary and reputable secondary links with dates.

Keep fact, interpretation, and forecast visibly separate. If the evidence is
balanced or weak, prefer a neutral or low-confidence conclusion.

## Completion Check

- The company, stock, or ETF identity and exchange are verified.
- The as-of time, forecast horizon, search windows, and data freshness are clear.
- Material recent news is dated, sourced, classified, and not duplicated.
- Company catalysts or ETF holdings and exposure paths are analyzed directly.
- Bullish, base, and bearish cases include triggers and invalidation signals.
- Scenario probability estimates are justified and total 100%.
- Any numerical move range has a stated evidence anchor.
- Facts, rumors, opinions, and forecasts are not conflated.
- The report discloses unavailable live data and avoids guarantees or
  personalized investment advice.
