# Antigravity Kit

> AI Agent templates with Skills, Agents, and Workflows

[![Antigravity Kit - Nổi bật trên Unikorn.vn](https://unikorn.vn/api/widgets/badge/antigravity-kit?theme=dark)](https://unikorn.vn/p/antigravity-kit?ref=unikorn)
[![Antigravity Kit - Hàng ngày](https://unikorn.vn/api/widgets/badge/antigravity-kit/rank?theme=dark&type=daily)](https://unikorn.vn/p/antigravity-kit?ref=unikorn)
[![Antigravity Kit on J2TEAM Launch](https://launch.j2team.dev/badge/antigravity-kit/dark)](https://launch.j2team.dev/products/antigravity-kit)

## Quick Install

```bash
npx @vudovn/ag-kit init
```

Or install globally:

```bash
npm install -g @vudovn/ag-kit
ag-kit init
```

This installs the `.agent` folder containing all templates into your project.

### ⚠️ Important Note on `.gitignore`

If you are using AI-powered editors like **Cursor** or **Windsurf**, adding the `.agent/` folder to your `.gitignore` may prevent the IDE from indexing the workflows. This results in slash commands (like `/plan`, `/debug`) not appearing in the chat suggestion dropdown.

**Recommended Solution:**
To keep the `.agent/` folder local (not tracked by Git) while maintaining AI functionality:

1. Ensure `.agent/` is **NOT** in your project's `.gitignore`.
2. Instead, add it to your local exclude file: `.git/info/exclude`

## What's Included

| Component     | Count | Description                                                        |
| ------------- | ----- | ------------------------------------------------------------------ |
| **Agents**    | 20    | Specialist AI personas (frontend, backend, security, PM, QA, etc.) |
| **Skills**    | 37    | Domain-specific knowledge modules                                  |
| **Workflows** | 11    | Slash command procedures                                           |

## Usage

### Using Agents

**No need to mention agents explicitly!** The system automatically detects and applies the right specialist(s):

```text
You: "Add JWT authentication"
AI: 🤖 Applying @security-auditor + @backend-specialist...

You: "Fix the dark mode button"
AI: 🤖 Using @frontend-specialist...

You: "Login returns 500 error"
AI: 🤖 Using @debugger for systematic analysis...
```

**How it works:**

- Analyzes your request silently

- Detects domain(s) automatically (frontend, backend, security, etc.)
- Selects the best specialist(s)
- Informs you which expertise is being applied
- You get specialist-level responses without needing to know the system architecture

**Benefits:**

- ✅ Zero learning curve - just describe what you need
- ✅ Always get expert responses
- ✅ Transparent - shows which agent is being used
- ✅ Can still override by mentioning agent explicitly

### Using Workflows

Invoke workflows with slash commands:

| Command          | Description                           |
| ---------------- | ------------------------------------- |
| `/brainstorm`    | Explore options before implementation |
| `/create`        | Create new features or apps           |
| `/debug`         | Systematic debugging                  |
| `/deploy`        | Deploy application                    |
| `/enhance`       | Improve existing code                 |
| `/orchestrate`   | Multi-agent coordination              |
| `/plan`          | Create task breakdown                 |
| `/preview`       | Preview changes locally               |
| `/status`        | Check project status                  |
| `/test`          | Generate and run tests                |
| `/ui-ux-pro-max` | Design with 50 styles                 |

Example:

```text
/brainstorm authentication system
/create landing page with hero section
/debug why login fails
```

### Using Skills

Skills are loaded automatically based on task context. The AI reads skill descriptions and applies relevant knowledge.

## CLI Tool

| Command         | Description                               |
| --------------- | ----------------------------------------- |
| `ag-kit init`   | Install `.agent` folder into your project |
| `ag-kit update` | Update to the latest version              |
| `ag-kit status` | Check installation status                 |

### Options

```bash
ag-kit init --force        # Overwrite existing .agent folder
ag-kit init --path ./myapp # Install in specific directory
ag-kit init --branch dev   # Use specific branch
ag-kit init --quiet        # Suppress output (for CI/CD)
ag-kit init --dry-run      # Preview actions without executing
```

## Documentation

- **[Web App Example](https://antigravity-kit-v2.vercel.app/docs/guide/examples/brainstorm)** - Step-by-step guide to creating a web application
- **[Online Docs](https://antigravity-kit-v2.vercel.app/docs)** - Browse all documentation online

## Buy me coffee

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/vudovn)

- or -

![Buy me coffee](https://img.vietqr.io/image/mbbank-0779440918-compact.jpg)

## License

MIT © Vudovn
