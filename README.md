📄 **[Read the Full 11-Page Whitepaper PDF Here](./LLM_Adversarial_Evaluation_Portfolio.pdf)**

# LLM Adversarial Evaluation

Structured adversarial evaluation of frontier LLMs, documenting reproducible failure modes across model families (Claude and GPT).

This is independent research conducted from 2025 to present. The goal is to probe frontier models on contested and underdetermined questions and document where their outputs fail in ways that are checkable from the transcript, not from the model's own self-report.

## Method

All findings are sorted with a four-category evidentiary rubric:

- **Checkable findings** — failures verifiable directly from the transcript
- **Ambiguous findings** — suggestive but not conclusive
- **Positive counter-examples** — cases where the model handled a hard prompt well
- **Confabulated introspection** — the model's explanations of its own behavior, treated as unverified color rather than proof

The work favors a small number of tight, transcript-verifiable findings over inflated counts. Descriptive claims are kept separate from causal ones. Model self-report is never load-bearing.

## Evaluation 1 — Claude (Anthropic)

Documented failure modes including:

- **Scope substitution** — narrowing or shifting the question actually asked
- **Strawmanning** — reframing a position into a weaker one before responding
- **Directionally consistent evidentiary errors** — mistakes that lean the same way rather than distributing randomly
- **Register-shift as a failure tell** — a change in tone or verbosity that correlates with lower-quality output

## Evaluation 2 — GPT (OpenAI)

Seven documented findings, including:

- **Fabricated source provenance** — citing sources that do not support the claim
- **Instruction violation after explicit agreement** — agreeing to a constraint, then breaking it
- **Asymmetric hedging** — hedging unevenly depending on the position taken
- **Certainty inflation** — expressing more confidence than the evidence supports
- **Extended scope substitution** — sustained drift from the original question across a session

## Tooling

Custom evaluation instructions that externalize self-monitoring checks, which reduced time-to-detection of recurring failure patterns within a session.

## Status

Full transcripts and worked examples available on request.
