# Run Examples

## Start MCP Server

From your project root:

```bash
python cdar/cdar_mcp.py
```

## Example Inference Modes

The exposed MCP tool is:

- `cdar_compositional_decomposed_adaptive_reasoning(image_path, question, force_strategy=None)`

If your caller supports passing `force_strategy`, current implementation accepts:

- Direct path:
  - `force_strategy="direct"`
- Decomposed path:
  - `force_strategy="decomposed"`
- Adaptive path:
  - Do not pass `force_strategy`

## Evaluation Suggestion

Run the same sample set across strategies:

1. direct
2. decomposed
3. adaptive (optional)

Then compare:

- answer accuracy
- average latency
- failure rate
- objective confidence fields in `reasoning` output
