# Stock monitoring watchlist

Requested on October 14, 2026 (America/Los_Angeles).

## Symbols

Preserve these user-supplied symbols and their order. Verify the issuer,
exchange, security type, and current listing status on each monitoring run;
do not silently replace ambiguous or inactive symbols.

| # | Symbol |
| --- | --- |
| 1 | COPX |
| 2 | EDU |
| 3 | GE |
| 4 | GEHC |
| 5 | GEV |
| 6 | GLD |
| 7 | NKE |
| 8 | RING |
| 9 | RVMD |
| 10 | SDOW |
| 11 | SLV |
| 12 | TIP |
| 13 | MSFT |
| 14 | AVNT |
| 15 | BEP |
| 16 | F |
| 17 | MBB |
| 18 | MRK |
| 19 | OGN |
| 20 | VOLT |
| 21 | XOM |

## Monitoring defaults

- News window: past seven calendar days, with older financial reports as context.
- Price windows: latest trading session, five trading sessions, and one month.
- Short-term outlook: 1-4 weeks.
- Long-term outlook: 6-12 months.
- Scenarios: base, bullish, and bearish for each horizon, with confirmation and
  invalidation signals.
- Evidence: dated sources, verified quote timestamps, consistent return
  adjustments, market and sector comparisons, and explicit missing-data notices.
- Baseline: first snapshot unless an actual previous report is supplied.

## Usage

In a skill-enabled Copilot chat:

> Use the stock-monitoring-research skill to monitor every symbol in
> watchlist.md. Include recent price and company developments, short-term and
> long-term scenarios, upcoming catalysts, and dated sources.

See the [monitoring skill](./.github/skills/stock-monitoring-research/SKILL.md)
for the full workflow. This file persists the requested watchlist, not a live
price feed or a research report. Monitoring runs on invocation; no schedule,
automatic alerts, or background service is configured.
