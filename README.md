# Strategic Popoltastic Deliverables

Claude Code plugin for producing branded deliverables for Strategic Popoltastic.

## Skills Included

| Skill | Command | Description |
|-------|---------|-------------|
| pdf | `/strategic-popoltastic:pdf` | Create branded PDFs |
| pptx | `/strategic-popoltastic:pptx` | Create branded presentations |
| docx | `/strategic-popoltastic:docx` | Create branded documents |
| xlsx | `/strategic-popoltastic:xlsx` | Create branded spreadsheets |
| proposal | `/strategic-popoltastic:proposal` | Build consulting proposals |
| remotion-video | `/strategic-popoltastic:remotion-video` | Create branded videos |
| press-release | `/strategic-popoltastic:press-release` | press-release |
| messaging-framework | `/strategic-popoltastic:messaging-framework` | messaging-framework |

## Installation

### Prerequisites

- Claude Code v2.1.49+ (with plugin support)
- Node.js 18+
- Python 3.11+ with [uv](https://docs.astral.sh/uv/) (for xlsx/pdf scripts)

### Setup

1. Add the private marketplace:
   ```
   /plugin marketplace add stromy-org/client-plugins-marketplace
   ```

2. Install the plugin:
   ```
   /plugin install strategic-popoltastic@stromy-org/client-plugins-marketplace
   ```

3. Install dependencies (first time only):
   ```bash
   cd ~/.claude/plugins/cache/strategic-popoltastic
   npm install
   uv sync
   ```

### Local Development

```bash
claude --plugin-dir /path/to/strategic-popoltastic-plugin
```

## Usage

Start Claude Code in any project directory and use the plugin skills:

- All output uses Strategic Popoltastic branding (colors, fonts, logo) automatically
- Skills are accessed as `/strategic-popoltastic:<skill-name>`

## Company Data

Brand data is in `companies/strategicpopoltastic/charter.json` and includes:
- Color palette (primary, secondary, accent)
- Typography (heading, body, monospace fonts)
- Logo files and paths

## Updating

```
/plugin update strategic-popoltastic
```

Or pull the latest version:
```bash
cd ~/.claude/plugins/cache/strategic-popoltastic
git pull
npm install
uv sync
```

## Version History

See [CHANGELOG.md](CHANGELOG.md) for version history.
