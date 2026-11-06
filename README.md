# CV Chap Chap resume skill for Claude

A Claude skill that helps you write a resume or CV from your real details, with the US resume rules built in
(one page, US Letter, no photo, no references, bullet points that start with a verb). It works on its own, and
with the free [CV Chap Chap](https://www.cvchapchap.com) connector it can also check your resume against real
rules, suggest a design and open the finished resume in the CV Chap Chap builder.

It never invents jobs, dates, numbers or skills: it asks, and leaves out what you do not give it.

## What is inside

- `cv-chap-chap/SKILL.md`: the skill. The same file is served at
  https://www.cvchapchap.com/.well-known/agent-skills/cv-chap-chap/SKILL.md.

## Install in Claude (claude.ai and the desktop app)

1. Download this repository as a ZIP (Code, then Download ZIP) and unzip it.
2. Zip the `cv-chap-chap` folder on its own.
3. In Claude, open Settings, then Capabilities, and upload that ZIP under Skills. Skills need code execution
   turned on.
4. Optional, for checks, designs and the finished resume: add the connector. Open
   [CV Chap Chap in Claude's connector directory](https://claude.ai/directory/connectors/cv-chap-chap), or add a
   custom connector in Settings, then Connectors, with `https://www.cvchapchap.com/mcp`. No account is needed.

Then ask: "Help me write a resume for a registered nurse job in Ohio."

## Install in Claude Code

```bash
git clone https://github.com/africanuspanga/cv-chap-chap-resume-skill
mkdir -p ~/.claude/skills
cp -R cv-chap-chap-resume-skill/cv-chap-chap ~/.claude/skills/
```

Add the connector as an MCP server if you want the tools:

```bash
claude mcp add --transport http cv-chap-chap https://www.cvchapchap.com/mcp
```

## What the connector does

| Tool | What it does |
|---|---|
| `check_cv` | Checks a resume against the CV Chap Chap builder's rules and lists what is missing or weak |
| `get_cv_format_guide` | CV conventions for a country |
| `find_cv_templates` | Suggests designs, with or without a photo |
| `save_cv_draft` | Saves the resume as a private draft and returns a link that opens it in the builder for 30 days |

Checks, guides and template searches are not stored. A saved draft is kept behind its link for 30 days; see
the [connector section of the privacy policy](https://www.cvchapchap.com/privacy#ai-connector).

Building, editing and previewing are free. Downloading the finished resume as PDF and Word is a one-time
payment, with no subscription.

## More

- How it fits together: https://www.cvchapchap.com/claude-resume-builder
- The connector: https://www.cvchapchap.com/ai-connector

## License

MIT. Made by [Driftmark Technologies Limited](https://www.driftmark.co.tz), the company behind CV Chap Chap.
