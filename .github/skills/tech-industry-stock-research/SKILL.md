---
name: tech-industry-stock-research
description: 'Research the latest tech industry news, hot topics, related companies, suppliers, and publicly traded stocks. Use when asked for technology investment themes, AI supply chains, semiconductor suppliers, data-center infrastructure, or a tech stock watchlist with current sources.'
argument-hint: 'Optional topic, region, exchanges, and as-of date'
---

# Tech Industry and Stock Research

Produce a current, source-backed industry briefing that connects technology
themes to companies, their suppliers, and publicly traded securities. This is
research, not a personalized investment recommendation.

## Scope

- Use the user's requested as-of date, or the current date when none is given.
  State it prominently in the report.
- Honor requested topics, regions, exchanges, and depth. Otherwise, cover the
  global technology industry and show US listings and relevant foreign listings.
- Research fresh information on every invocation. Do not reuse a previous
  report's news, financial figures, supplier relationships, or listing status
  without checking them again.
- Do not create report files, modify the workspace, or commit unless requested.

## Workflow

### 1. Identify current themes

1. Use available web search and page-reading tools to find recent technology
   news, company announcements, and financial results.
2. Start with the past 30 days; expand to 90 days or older material when needed.
   Label older sources as background rather than current news.
3. Choose three to five themes supported by the evidence, and identify the
   strongest theme. Explain the ranking using adoption, actual revenue,
   capital spending, deployment progress, or supply constraints, rather than
   headlines alone.
4. Consider AI agents, inference, custom chips, semiconductor manufacturing,
   memory, networking, power, cooling, cybersecurity, and robotics as possible
   themes, not a fixed conclusion.

### 2. Verify evidence

- Prefer company investor relations, earnings releases, filings, official
  technical announcements, and stock exchanges. Use reputable independent
  reporting for context and corroboration.
- Open the original sources for material claims. Search summaries and generated
  answers are leads, not proof. Record the publication date and the period or
  event date to which each claim refers.
- Never cite material published after the as-of date as evidence available then.
  For historical reports, exclude later revisions that introduce hindsight.
- Distinguish achieved results from forecasts, samples, qualification,
  production, previews, planned deployment, and nonbinding agreements.
- Distinguish fiscal years from calendar years, and quarterly figures from
  annual figures. Keep currencies, units, and comparison periods explicit.
- If a page is blocked or unavailable, try another public primary source or
  reputable corroborating report. Disclose remaining verification limitations;
  omit unsupported figures and do not invent URLs, dates, or news.
- Describe important conflicts between sources instead of silently resolving
  them. Do not repeat unverified supply allocations or market-share estimates.

### 3. Map companies and the supply chain

1. Identify the companies building, buying, operating, or monetizing each theme.
2. Trace relevant inputs: manufacturing, packaging, memory, components,
   networking, equipment, software, power, and cooling, as appropriate.
3. Verify each named buyer-supplier connection separately. Providing a relevant
   product is not proof that a company supplies a particular buyer.
4. Classify each relationship as a confirmed direct supplier, announced
   development partner, operator-facing infrastructure vendor, upstream
   supplier, competitor, or broader industry exposure.
5. For planned or reported relationships, state that status explicitly. Do not
   label an ecosystem partner or a competitor as a direct supplier.
6. Cite the evidence next to the relationship or use numbered references that
   unambiguously map each relationship to its source.

### 4. Verify stocks and listings

- Check company names, ticker symbols, exchanges, and current listing status
  using official investor or exchange information where available.
- Show the exchange with every ticker. Distinguish ordinary shares, ADRs, and
  different share classes when relevant.
- For a private company or an unconfirmed listing, say there is no verified
  publicly tradable ticker. Do not invent symbols or treat IPO rumors as a
  completed listing.
- Explain that investing in a public supplier, partner, or shareholder gives
  indirect exposure, not direct ownership of a private company.
- Include prices only if requested and verified. State their currency,
  timestamp, and whether they are delayed. Never imply the report contains
  live prices when it does not.

### 5. Present the briefing

Use this structure, adapting the number of rows to the requested scope:

1. **As-of date and bottom line:** the strongest topic and why it matters.
2. **Hot topics:** topic, catalyst, evidence date, and source.
3. **Main companies:** company, role, related topic, exchange, and ticker or
   private/unverified status.
4. **Suppliers and partners:** company, product or service, named buyer,
   relationship classification, exchange/ticker, and supporting source.
5. **Watchlist by exposure:** group the listed stocks by software/adoption,
   compute, manufacturing/components, or infrastructure as appropriate.
6. **Risks and limitations:** valuation, monetization, cyclicality, customer
   concentration, competition, execution, regulation, and geography where
   relevant. Separate factual findings from investment interpretation.

Keep the report readable and concise, with clickable source links. A popular
theme is not evidence that its related stocks are attractively priced.

## Completion Check

- The as-of date and source dates are clear, with no future-dated evidence.
- Material developments and buyer-supplier links have supporting citations.
- Announcements and forecasts are not presented as operating results.
- Tickers, exchanges, listing status, and security types have been checked.
- Direct suppliers are separated from partners and indirect exposure.
- Missing verification and any absence of live pricing are disclosed.
- The report answers all four questions: hot topics, companies, suppliers,
  and related publicly traded stocks.
