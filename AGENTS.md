> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links

## Terminology

- **Classroom Hub / DV Edu** — school classroom platform at `edu.daven.ai` (`dv-edu` repo)
- **Education app / Edu app** — hosted lesson tool embedded in Edu via iframe (not the Hub itself)
- **MCP proxy** — Edu Nest path `/api/v1/mcp-proxy` that education apps call with a session (no browser API keys)
- Prefer "education app" / "교육앱" over vague "MCP app" in end-user docs; "MCP app" is fine in technical contract pages

Developer docs for Edu apps live under `edu/` (KO) and `en/edu/` (EN), tab **교육앱 개발** / **Edu Apps**.

Machine-readable Edu contract (prefer for coding agents):

- `edu/llms.txt` / `en/edu/llms.txt`
- `edu/openapi.yaml`
- `edu/agent-spec.mdx` / `en/edu/agent-spec.mdx`

Prefer Mintlify components (`Card`, `Columns`, `Steps`, `Tabs`, `CodeGroup`, `Accordion`, callouts) on Edu pages — keep them scannable, not long prose.

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Prefer product-facing developer docs; skip undocumented internal admin features unless asked
