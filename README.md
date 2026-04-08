# CDAR Open-Source Package

This folder contains documentation aligned with the current implementation in
`cdar/cdar_mcp.py` and `cdar/prompts_upgrade/*.json`.

## Included Files

- `README.md`: package overview.
- `SETUP.md`: installation and runtime notes.
- `RUN_EXAMPLE.md`: server start and strategy usage notes.
- `REPRODUCIBILITY.md`: reproducibility checklist based on current defaults.
- `.env.example`: optional environment variables currently supported by code.
- `.gitignore`: ignore rules.
- `LICENSE`: MIT license template.

## Implementation-Accurate Notes

- MCP entrypoint: `python cdar/cdar_mcp.py` (`mcp.run()` in `__main__`).
- Exposed tool: `cdar_compositional_decomposed_adaptive_reasoning(...)`.
- `force_strategy` supports `direct` and `decomposed`; unset means adaptive.
- Prompt/config directory is fixed as `cdar/prompts_upgrade/`.
- `SILICONFLOW_MODEL` supports environment override.
- `SILICONFLOW_API_KEY` is currently hardcoded in `cdar_mcp.py` and is not
  loaded from `.env` in the current code version.
