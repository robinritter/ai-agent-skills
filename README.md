# AI Agent Skills & Prompts — Robin the Quant

Practical AI agent skills and copy-and-paste prompts for crypto research, portfolio
risk, market news and trading decisions. Every workflow explains its findings in
**Robin the Quant's** voice: direct, evidence-led and skeptical of hype.

Start with a real question. Get transparent reasoning, sources where needed and
an honest account of what the evidence cannot establish.

## Choose a skill

| Skill | What you get | Example request |
|---|---|---|
| [Crypto fundamental analysis](skills/crypto-fundamental-analysis/SKILL.md) | Complete 18-point project report, tokenomics, security, unlocks and peer valuation | “Analyze [project + official link] using the full framework.” |
| [Portfolio risk analysis](skills/portfolio-risk-analysis/SKILL.md) | Concentration, shared exposure and BTC −30% / −50% crash scenarios | “Here are my holdings. Show me the concentration and crash scenarios.” |
| [Market signal triage](skills/market-signal-triage/SKILL.md) | News classified by decision relevance, with at most three next checks | “Sort these headlines for my holdings over the next week.” |
| [Trade thesis challenger](skills/trade-thesis-challenger/SKILL.md) | Strong opposing case, possible biases and testable invalidation | “Pressure-test this sell decision and my reasoning.” |

The three [Fable prompt editions](prompts/fable/README.md) can be copied directly
into an AI chat. The skills provide the same workflows in reusable `SKILL.md` form.

## Use a skill

1. Download or clone this repository:

   ```sh
   git clone https://github.com/robinritter/ai-agent-skills.git
   ```

2. Choose one folder under `skills/`. Give your AI agent its `SKILL.md` and all
   bundled references, or install that entire folder through your agent's supported
   skill-installation workflow. Each skill is self-contained; preserve its relative
   file structure. The repository root itself is not a skill.
3. Ask your question with the inputs listed in the skill. For an agent without a
   skill loader, explicitly ask it to read and follow the selected `SKILL.md` and
   its linked references. For a copy-and-paste chat, use a Fable prompt edition.

A capable language model is required. Current project research and news verification
also require browsing that can open sources. Image inputs require vision or a typed
transcription. Paid APIs, a private research library and wallet access are not
required. If a provider is blocked or a number is missing, the workflow reports the
coverage gap rather than inventing it. Installation/discovery varies by client;
this repository does not claim every agent automatically follows the instructions.

## The fundamental-analysis report

The [full format](skills/crypto-fundamental-analysis/references/report-template.md)
preserves the original 18 sections: problem, market, team, investors, product,
technology, security, tokenomics, utility, unlocks, business model, competition,
partnerships, community, development, liquidity, valuation and risks.

It includes a quick rating card, executive summary, findings/pros/cons/sources,
bull and bear cases, catalysts, risk assessment, Robin's research verdict, major
red flags, competitor comparison and sources. The score has a transparent rubric;
material missing evidence produces “not rated.” The verdict is Consider, Wait,
Avoid or Hold/reassess for an existing holder, with explicit conditions.

## Evidence over confidence

Portfolio weight is not a measured share of risk. Hypothetical beta scenarios are
not forecasts. Old headlines do not prove markets have fully priced them in.
Missing a price stop does not prove an emotional trade. Audits, named investors
and high scores cannot establish safety or future returns.

These skills support research and decisions. They do not execute trades, connect
wallets or determine an individual's suitable allocation. Never provide seed
phrases or account credentials.

## Examples, checks and contribution

See [worked scenarios](examples/scenarios.md) and [evaluation cases](evals/README.md).
Structural validation and manual scenario checks are distinct from a live market
research run. Fresh-client discovery and independent model testing are not yet
verified. See [release validation](evals/release-validation.md).

To contribute, extend the existing skill that owns the job. Keep its trigger,
inputs, source requirements, failure behavior and output explicit. Bundle referenced
files and test a valid request, missing input and a near-miss. Keep credentials,
private portfolios and private course material out of commits. Update the matching
Fable copy edition when changing its canonical skill.

## License

[MIT](LICENSE). Data providers and linked sources retain their own terms.
