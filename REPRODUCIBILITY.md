# Reproducibility Checklist

## Core Run Configuration

- Model endpoint/provider: SiliconFlow chat completions API
- Model name default: `Qwen/Qwen3-VL-32B-Instruct`
- API temperature default: `0.0` (direct decomposition/reasoning calls may override)
- Seed default: `42`
- Max tokens: `2048`
- Timeout/retry: timeout `120s`, retries `3`

## CDAR Configuration Snapshot

- `cdar/prompts_upgrade/system_config.json`: version `1.0`, output version `1.2-optimized`
- `cdar/prompts_upgrade/decomposition.json`
- `cdar/prompts_upgrade/reasoning.json`
- `cdar/prompts_upgrade/strategy_rules.json`
- `cdar/prompts_upgrade/complexity_rules.json`
- `cdar/prompts_upgrade/question_types.json`
- `cdar/prompts_upgrade/defaults.json`
- `cdar/prompts_upgrade/correction.json`
- `cdar/prompts_upgrade/subtask_types.json`
- `cdar/prompts_upgrade/refinement.json`

## Experiment Protocol

- Dataset split:
- Number of samples:
- Evaluation metric(s):
- Forced strategy settings (tool argument `force_strategy`):
  - direct
  - decomposed
  - adaptive (optional)

## Logging Requirements

- Save raw predictions per sample.
- Save parsed final answers.
- Save run timestamp.
- Save average latency and failure counts.
- Save strategy used (`adaptive_strategy`) and decomposition payload.

## Minimal Ablation Table

| Strategy | Accuracy | Avg Latency | Notes |
|---|---:|---:|---|
| direct |  |  |  |
| decomposed |  |  |  |
| adaptive (optional) |  |  |  |
