# GitHub Copilot Instructions

## Project Overview
This repository belongs to **JORDANA-KRAKATAMI-ORG**. These instructions guide GitHub Copilot on how to assist with development in this codebase.

---

## Tech Stack & Preferences

- **Languages:** TypeScript / JavaScript, SQL/PostgreSQL, Bash/Shell, Python
- **Frameworks:** React, Node.js
- **Infrastructure:** Docker, Cloudflare Workers, Railway, Hostinger VPS
- **Databases:** PostgreSQL (Supabase), prefer parameterized queries always
- **Automation:** n8n workflows, API-first integrations
- **Package manager:** npm or pnpm preferred

---

## Coding Standards

### General
- Write clean, readable, and self-documenting code
- Prefer explicit types over `any` in TypeScript
- Use `async/await` over `.then()` chains
- Always handle errors explicitly — never swallow exceptions silently
- Keep functions small and single-purpose
- Prefer immutable data patterns where possible

### TypeScript / JavaScript
- Use strict TypeScript settings (`"strict": true`)
- Prefer `const` over `let`; avoid `var`
- Use named exports over default exports for utilities and components
- Use descriptive variable names — avoid abbreviations unless standard (e.g., `req`, `res`, `err`)
- Add JSDoc comments for exported functions and complex logic

### SQL / PostgreSQL
- Always use parameterized queries to prevent SQL injection
- Use migrations for schema changes — never alter production schema manually
- Prefer `snake_case` for table and column names
- Add indexes on foreign keys and frequently queried columns

### Bash / Shell
- Use `#!/usr/bin/env bash` shebang
- Use `set -euo pipefail` for safety
- Quote all variables: `"${VAR}"`
- Add comments for non-obvious logic

---

## API & Integration Patterns
- Use environment variables for all secrets and API keys — never hardcode credentials
- Validate and sanitize all external input
- Return consistent error responses: `{ error: string, code?: string }`
- Log errors with context, not just the message
- Use retry logic with exponential backoff for external API calls

---

## File & Project Structure
- Group by feature/domain, not by file type
- Place shared utilities in `/lib` or `/utils`
- Keep configuration in `/config` or environment files
- Name files in `kebab-case`

---

## Security
- Never commit secrets, tokens, or passwords
- Sanitize user input before DB writes or rendering
- Use HTTPS for all external connections
- Apply principle of least privilege for service accounts and API keys

---

## Pull Request Guidelines
- Keep PRs focused and small — one concern per PR
- Write descriptive PR titles: `feat:`, `fix:`, `chore:`, `refactor:` prefixes
- Include a brief description of what changed and why
- Reference related issues when applicable

---

## Comments & Documentation
- Explain *why*, not *what* — the code shows what, comments explain the reasoning
- Mark TODOs with: `// TODO(owner): description`
- Keep README files up to date with setup and usage instructions
