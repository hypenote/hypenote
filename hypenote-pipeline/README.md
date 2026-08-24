# Hypenote Reference Pipeline

> 🚧 **Work in progress**

This directory is reserved for the Hypenote reference implementation for:

**audio → transcription → speakers → transcript enrichment → LLM analysis → structured output**

## Goals

- Local-first default path
- English-first benchmarked defaults
- Audio-file-first ingestion
- Model-swappable STT / diarization / LLM adapters
- Hypenote bookmark preservation
- Timestamp-linked evidence
- Markdown + JSON outputs
- No required cloud account
- Reproducible benchmarks

## Proposed first milestone

```text
input.wav / input.m4a
    ↓
normalize
    ↓
ASR
    ↓
timed transcript
    ↓
optional diarization
    ↓
local LLM
    ↓
summary.md
transcript.json
analysis.json
```

## Planned modules

```text
ingest/
audio/
stt/
diarization/
transcript/
analysis/
prompts/
schemas/
exports/
benchmarks/
```

## Evaluation

The first benchmark should focus on conversational English and report:

- normalized WER
- named-entity accuracy
- speaker-attribution quality
- timestamp drift
- hallucinations during silence/noise
- real-time factor
- RAM / VRAM usage
- summary factuality

The implementation is intentionally not committed to one ASR model yet. Parakeet, Canary and the Whisper ecosystem are all worth testing on the same Hypenote recordings.
