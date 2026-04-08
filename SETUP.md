# Setup Guide

## 1) Python Environment

```bash
python -m venv .venv
```

Activate environment:

- Windows PowerShell:
```powershell
.venv\Scripts\Activate.ps1
```

## 2) Install Dependencies

From project root:

```bash
pip install -r requirements.txt
```

## 3) Runtime Configuration Notes

- `cdar/cdar_mcp.py` reads prompt/config JSON from:
  - `cdar/prompts_upgrade/`
- Required JSON files in current implementation:
  - `system_config.json`
  - `defaults.json`
  - `decomposition.json`
  - `reasoning.json`
  - `question_types.json`
  - `correction.json`
  - `complexity_rules.json`
  - `strategy_rules.json`
  - `subtask_types.json`
  - `refinement.json`

## 4) Environment Variables (Current Code Behavior)

- Supported by current code:
  - `SILICONFLOW_MODEL` (optional override)
- Not yet read from env in current code:
  - `SILICONFLOW_API_KEY` (currently hardcoded in `cdar/cdar_mcp.py`)

## 5) Validate

- Ensure image paths are valid.
- Ensure prompt JSON files exist in `cdar/prompts_upgrade/`.
