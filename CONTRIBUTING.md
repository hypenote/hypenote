# Contributing

Thanks for helping improve this map of private audio intelligence pipelines.

## Add a project

A strong candidate should cover **transcription plus at least one downstream intelligence layer**, such as:

- speaker diarization / attribution,
- transcript cleanup or enrichment,
- summaries,
- decisions / action items,
- transcript Q&A,
- search / RAG,
- agent or MCP integration.

Projects that only wrap Whisper with no downstream analysis may still be useful, but normally belong in **Other projects worth watching** rather than the Top 10.

## What to include in a PR

Please provide:

1. Repository URL
2. Short description
3. Supported audio inputs
4. ASR backend(s)
5. Speaker diarization / attribution approach
6. LLM providers or local-model support
7. Privacy model
8. Supported platforms
9. License
10. Why it is useful for an English-first private pipeline
11. Any important maintenance, security or licensing caveats

## Ranking philosophy

The Top 10 is not ranked by stars alone. We prioritize:

- end-to-end completeness,
- English transcription quality potential,
- privacy and local execution,
- speaker handling,
- LLM flexibility,
- architecture reusability,
- documentation and maturity,
- license clarity.

If you disagree with a ranking, a PR with reproducible evidence is more useful than a popularity argument.

## Benchmarks

Benchmark contributions are especially welcome.

Useful test categories include:

- meetings,
- interviews,
- lectures,
- noisy rooms,
- multiple English accents,
- names and technical vocabulary,
- long recordings,
- silence / false-positive hallucinations,
- multi-speaker overlap.

Please document hardware, model version, decoding settings and evaluation method.
