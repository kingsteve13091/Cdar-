# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| main    | ✅        |

## Reporting a Vulnerability

If you discover a security vulnerability in CDAR, **please do not open a public issue**.

Instead, contact the maintainer privately:

- Email: *(add your email here)*
- Or use [GitHub Security Advisories](../security/advisories/new) (recommended).

We will acknowledge receipt within 48 hours and aim to provide a fix or mitigation within 7 days.

## Known Security Considerations

- `SILICONFLOW_API_KEY` is currently hardcoded in `cdar_mcp.py`. Contributors should never commit real API keys. Use a placeholder value and document the replacement step.
- The MCP server accepts local file paths as input. Ensure it is not exposed to untrusted networks without additional access controls.
