# LLM Settings

This repository contains configuration settings for various LLM tools, primarily Claude Code.

## Contents

- `claude/settings.json` - Claude Code configuration settings
- `CLAUDE.md` - Instructions for Claude Code when working with this repository

## Claude Code Settings

The settings file includes:

### Security & Permissions
- Carefully curated allow/deny lists for file operations and commands
- Protection against destructive operations and credential access
- Restricted network operations for security

### Privacy
- Telemetry disabled
- Error reporting disabled
- Non-essential traffic disabled

### Configuration
- Model: Sonnet (Claude 3.5)
- MCP servers enabled
- Extended API timeout (10 minutes)
- Auto-updates disabled

## Usage

To use these settings with Claude Code:

1. Create a symbolic link from this repository to your project:
   ```bash
   ln -s /path/to/llm-settings/claude /path/to/your-project/.claude
   ```
2. Alternatively, copy `claude/settings.json` to your project's `.claude/` directory
3. Adjust permissions as needed for your specific project
4. Review and modify environment variables if required

## Customization

When modifying settings:
- Always validate JSON syntax
- Test permission changes in a safe environment
- Document changes in commit messages
- Review security implications of permission changes

## License

MIT
