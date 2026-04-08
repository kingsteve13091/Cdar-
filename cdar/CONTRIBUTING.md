# Contributing to CDAR

Thank you for your interest in contributing to CDAR!

## How to Contribute

### Reporting Issues

- Use [GitHub Issues](../issues) to report bugs or request features.
- Include: Python version, OS, error traceback, and steps to reproduce.

### Submitting Changes

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/your-feature`.
3. Make your changes and ensure the MCP server starts without errors.
4. Commit with a clear message: `git commit -m "Add: description of change"`.
5. Push and open a Pull Request against `main`.

### Code Style

- Follow existing code conventions in `cdar_mcp.py`.
- Use type hints for function signatures.
- Keep configuration in `prompts_upgrade/*.json`; avoid hardcoding values in Python.

### What We Accept

- Bug fixes with clear reproduction steps.
- New question-type support or strategy improvements.
- Documentation improvements.
- Test coverage additions.

### What Requires Discussion First

- Architectural changes (e.g., replacing FastMCP, changing the pipeline phases).
- New external dependencies.
- Changes to the output JSON schema.

Please open an issue before starting work on these.

## Code of Conduct

Be respectful and constructive. We follow the spirit of the [Contributor Covenant](https://www.contributor-covenant.org/).
