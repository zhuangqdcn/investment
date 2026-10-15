# investment

## Company incident and stock impact research skill

[company-incident-stock-research](./.github/skills/company-incident-stock-research/SKILL.md)
is a reusable Copilot skill for scanning recent news for events that could
materially help or hurt large public-company stocks, especially safety
incidents, scandals, recalls, cyberattacks, outages, and regulatory actions.

In a skill-enabled Copilot chat, invoke `/company-incident-stock-research` or ask:

> Check the past seven days for major company incidents like the United Express
> passenger removal or Boeing 737 MAX groundings, plus positive catalysts.
> Show company names, stock symbols and exchanges, verified sources, reported
> stock reactions, potential impact size and duration, and reversal risks.

Optionally specify the news window, as-of date, companies, sectors, exchanges,
or impact horizon. The skill distinguishes fresh developments from recycled
news, checks recovery updates, and separates observed price moves from future
scenarios. It avoids unsupported percentage forecasts and does not provide
personalized investment advice.

## Company and ETF news-move research skill

[company-etf-news-move-research](./.github/skills/company-etf-news-move-research/SKILL.md)
is a reusable Copilot skill for checking recent news about a specified public
company, stock, or ETF and assessing plausible price moves.

In a skill-enabled Copilot chat, invoke `/company-etf-news-move-research` or ask:

> Check all recent news for NVDA or QQQ and assess the possible moves over the
> next one to four weeks. Include verified sources, bullish, base, and bearish
> scenarios, probability estimates, catalysts, and invalidation signals.

Optionally specify the security name or ticker, exchange, forecast horizon,
market, or an as-of date. The skill verifies the security and current sources,
distinguishes new information from priced-in context, and analyzes ETF holdings
and exposure paths where relevant. It uses evidence-based scenarios rather than
guaranteed predictions and does not provide personalized investment advice.

## Stock monitoring research skill

[stock-monitoring-research](./.github/skills/stock-monitoring-research/SKILL.md)
is a reusable Copilot skill for monitoring a company or stock watchlist,
explaining recent price and business developments, and assessing separate
short-term (1-4 weeks) and long-term (6-12 months) outlooks.

In a skill-enabled Copilot chat, invoke `/stock-monitoring-research` or ask:

> Monitor AAPL, MSFT, and NVDA. Show recent price movements and company news,
> compare performance with market and sector benchmarks, and give short-term
> and long-term base, bullish, and bearish scenarios. Include dated sources,
> upcoming catalysts, and evidence that would change each outlook.

Optionally specify exchanges, an as-of date, news and forecast windows, or a
previous report. Supplying a previous report lets the skill highlight new,
changed, and resolved developments. Without one, it creates a first snapshot.
Unavailable market data is disclosed rather than invented, and forecasts are
conditional research rather than guaranteed returns or personalized advice.

The skill refreshes research when invoked; it does not continuously monitor,
save state, schedule runs, or send alerts on its own. Recurring monitoring
requires a separately configured scheduler and data access.

## Biotech drug and stock research skill

[biotech-drug-stock-research](./.github/skills/biotech-drug-stock-research/SKILL.md)
is a reusable Copilot skill for researching cancer drugs and other active
disease areas, mapping companies to stock symbols, and evaluating clinical
evidence alongside Reddit and public patient-community discussions.

In a skill-enabled Copilot chat, invoke `/biotech-drug-stock-research` or ask:

> Research the latest cancer, obesity, Alzheimer, MASH, and autoimmune drug
> developments. Include company stock symbols, clinical trial and approval
> status, verified Reddit or patient-community reports, potential outcomes,
> upcoming catalysts, and dated primary sources.

Optionally specify diseases, drugs, companies, exchanges, a research horizon,
or an as-of date. The skill refreshes sources each time, separates patient
anecdotes from trial evidence, and distinguishes trial success, regulatory
approval, commercial success, and stock returns. It avoids unsupported
approval probabilities and does not provide personalized medical or
investment advice.

## Technology industry research skill

[tech-industry-stock-research](./.github/skills/tech-industry-stock-research/SKILL.md)
is a reusable Copilot skill for researching current technology themes, related
companies, verified supplier relationships, and publicly traded stocks.

In a skill-enabled Copilot chat, invoke `/tech-industry-stock-research` or ask:

> Research the latest tech industry hot topics, the companies involved, their
> suppliers, and related stocks. Include dated sources and exchange/ticker
> symbols.

Optionally specify a topic, region, exchanges, or an as-of date. The skill
refreshes its sources each time, distinguishes confirmed suppliers from
partners and indirect exposure, and flags verification gaps. It does not
provide live stock prices unless requested and verified, or personalized
investment recommendations.

## Geopolitical market research skill

[geopolitical-market-research](./.github/skills/geopolitical-market-research/SKILL.md)
is a reusable Copilot skill for checking current world politics, evaluating
possible conflicts and US policy moves, and mapping their effects to stocks
and commodities.

In a skill-enabled Copilot chat, invoke `/geopolitical-market-research` or ask:

> Check the latest world politics. Assess the next plausible conflicts or US
> policy moves over 3-12 months, and explain which stocks and commodities could
> benefit or suffer. Include dated sources, alternative scenarios, and the
> evidence that would change the outlook.

Optionally specify a region, conflict, investment horizon, exchanges,
commodities, or an as-of date. The skill verifies underlying sources,
distinguishes facts from forecasts, and explains both escalation and
de-escalation risks. Its watchlist is research, not a buy signal; live prices
and valuations are not assumed to have been checked.
