---
name: biotech-drug-stock-research
description: 'Research current cancer drugs and other hot disease areas, biotech stocks, clinical trial results, approval prospects, and Reddit or patient-community reports. Use for oncology, obesity, diabetes, Alzheimer disease, MASH, autoimmune therapies, drug pipelines, trial catalysts, and evidence-based biotech watchlists.'
argument-hint: 'Disease, drug, company, exchanges, research horizon, or as-of date'
---

# Biotech Drug and Stock Research

Build a dated, source-verified drug-development watchlist and compare formal
clinical evidence with public patient experiences and investor discussion.
Refresh the research on every invocation; do not treat previous chat summaries
or example tickers as current evidence.

## Scope

- Use the diseases, companies, and markets requested by the user. If expanding
  broadly, start with oncology, obesity and diabetes, Alzheimer disease, MASH
  (formerly NASH), and autoimmune disease; add other areas only when current
  evidence supports their relevance.
- State the as-of date, news window, geography, and assumptions. Default to
  the past 30 days for news, using older pivotal evidence with its actual date.
- Cover public-company exposure, clinical and regulatory status, potential
  catalysts, community observations, and reasons the investment thesis could
  fail. Do not equate a hot disease area with an attractive stock valuation.
- Do not create report files, modify the workspace, commit, or push unless
  explicitly requested.

## Workflow

### 1. Discover developments and verify original sources

1. Search current drug news and identify a bounded set of relevant programs.
   Include setbacks and negative results, not only positive announcements.
2. Open original regulator announcements, trial registries, peer-reviewed
   publications, conference abstracts, and company releases when available.
   Use independent reporting for context, not as a substitute for an
   accessible primary source.
3. Treat search-generated summaries and citations as leads. Check the actual
   page, title, date, and content before relying on a claim or linking a post.
   Never manufacture plausible URLs, forum titles, dates, or results.
4. Separate publication date, data cutoff, trial completion, and anticipated
   readout dates. Exclude developments after the requested as-of date.
5. Explicitly disclose access failures, stale evidence, conflicting sources,
   and unavailable results. A failed search is not proof no discussion or
   update exists. Try another public source or a browser when appropriate,
   without bypassing access controls or entering private communities.

### 2. Map drug ownership and publicly traded exposure

1. Verify the developer, license holder, parent, and commercial partners.
   Distinguish the drug name from a stock symbol and a subsidiary from its
   publicly listed parent.
2. Verify each ticker, exchange, country, and share type against company
   investor relations or an exchange. Clearly distinguish primary listings,
   ADRs, OTC securities, and market-data suffixes.
3. Explain shared economics only when supported by licensing or partnership
   evidence. Do not infer equal exposure from a combination regimen.
4. Distinguish diversified pharmaceutical companies from concentrated
   development-stage companies. Note financing, dilution, manufacturing, and
   execution risks when relevant. Verify cash runway or valuation figures
   from dated filings if reporting them; do not assume live prices.

### 3. Establish clinical and regulatory status

1. Record the indication, biomarker restrictions, line of therapy, formulation,
   phase, registry identifier, design, comparator, and population size.
2. Distinguish planned, recruiting, completed, and reported studies; a trial
   launch or regulator agreement is not a successful trial.
3. Distinguish investigational drugs, submitted applications, accepted
   applications, accelerated or conditional approvals, full approvals, and
   new indications or combinations of existing drugs. Specify jurisdiction.
   Fast Track or Breakthrough Therapy designation is not approval.
4. Report the primary endpoint, effect size, comparator result, uncertainty
   intervals or significance where available, follow-up, and major safety
   findings. Label company topline results, exploratory subgroups, and
   unconfirmed responses accurately.
5. Keep endpoints distinct: tumor response is not survival; amyloid removal
   is not cognitive benefit; liver-biopsy improvement is not proven prevention
   of clinical complications. Explain immature or nonsignificant survival data.
6. For weight-loss data, specify duration, dose, population, placebo adjustment,
   and estimand when available. Do not rank treatments using incomparable
   cross-trial percentages. Keep oral and injectable evidence separate.
7. Include adverse-event discontinuations and serious toxicities, not just
   efficacy. Do not extrapolate small cohorts to population-level safety.

### 4. Check Reddit and other public user-based communities

1. Search drug names, aliases, company names, and tickers in relevant disease,
   trial-participant, and investor communities. Prefer patient or caregiver
   discussions for experience and investor forums for sentiment.
2. Open specific threads and relevant comments. A subreddit homepage, search
   snippet, or reposted press release is not verified patient testimony.
   If search indexing is weak, try the site's public search in a browser.
3. For each cited observation, provide the direct thread URL, verified title,
   date or explicitly approximate displayed age, and a concise paraphrase.
   Distinguish the original post from later updates and comments. Do not
   reproduce usernames or unnecessary identifying health details.
4. Label first-person or caregiver accounts as unverified self-reports.
   Separate clinical-trial participation from use of unapproved or
   gray-market products whose identity, purity, or dosing cannot be verified.
   Do not recommend suppliers, sourcing, or unsupervised treatment.
5. Look for both favorable and unfavorable experiences: tolerability,
   discontinuation, durability, relapse or regain, access, insurance, and
   treatment burden. Identify investor speculation and news aggregation.
6. State the small, nonrepresentative nature of the reviewed sample. Account
   for selection, survivorship, reporting, placebo, and promotional biases.
   In blinded trials, perceived benefit does not establish treatment assignment.
7. Cross-check themes with formal evidence. Do not count forum reports as an
   independent efficacy dataset, infer adverse-event rates, or translate
   enthusiasm into an approval probability. If no substantive thread is
   verified, say so without claiming none exists.

### 5. Assess possible outcomes without false precision

1. Separate four questions: will the study meet its endpoint, will regulators
   approve the specific indication, will the product succeed commercially,
   and will shareholders benefit at the current valuation?
2. Explain favorable evidence and failure modes: study size and controls,
   endpoint relevance, effect durability, replication, safety, missing data,
   manufacturing, regulatory requirements, and competitive alternatives.
3. Default to qualitative evidence maturity and uncertainty, explaining the
   basis. For already-approved uses, discuss remaining confirmatory,
   expansion, safety, or commercial questions rather than pending first
   approval. Do not assign an arbitrary drug-specific percentage.
4. If numerical probabilities are requested, use a transparent, documented
   method with assumptions and sensitivity analysis, or state that the
   evidence is insufficient. Historical success rates must have a verified
   source, disease category, time period, and denominator; distinguish
   single-phase transitions from cumulative likelihood of approval.
   Never equate an observed response rate with an approval probability.
5. Present evidence-based favorable, base, and unfavorable scenarios when
   useful, plus the next verified milestone and evidence that would change
   the outlook. Label company guidance and avoid inventing readout dates.

## Presentation

1. Start with the as-of date, scope, main findings, and material verification
   gaps.
2. Provide a watchlist table with disease, drug, company, ticker/exchange,
   status, dated evidence, next milestone, and key risks. Attach sources close
   to claims; use a source key if needed to keep the table readable.
3. Provide community checks with direct threads, approximate ages only when
   necessary, what users reported, evidence type, and what cannot be inferred.
4. Summarize evidence maturity and potential outcomes separately from stock
   exposure. Explain catalysts, competition, access, and dilution without
   presenting the watchlist as a buy recommendation.
5. Clearly state that this is research, not individualized investment or
   medical advice. Do not promise trial success, cures, or stock returns.

## Completion Check

- All material facts have accessible supporting sources or explicit gaps.
- Dates, stages, indications, and regulatory jurisdictions are distinguished.
- Ownership, tickers, exchanges, and security types are verified.
- Results include denominators, comparators, limitations, and relevant safety.
- Community links were opened; anecdotes and speculation are labeled.
- No false precision, unsupported future dates, or misleading comparisons.
- Trial success, approval, commercial outcomes, and returns remain separate.
