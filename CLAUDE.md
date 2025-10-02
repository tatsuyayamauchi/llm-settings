# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This repository stores LLM configuration settings, specifically Claude Code settings.

## Repository Structure

- `claude/settings.json` - Claude Code settings configuration file

## Settings Overview

The `claude/settings.json` file contains:

### Permissions
- **Allowed operations**: File reading, writing to src/docs/.tmp, essential git commands, package installation, basic file operations
- **Denied operations**: Privileged operations (sudo), destructive commands, credential access, network operations, destructive git operations

### Model Configuration
- Default model: Sonnet
- MCP servers: Enabled for all project servers

### Environment Variables
- Telemetry and error reporting: Disabled
- API timeout: 600 seconds
- Auto-updater: Disabled

## Working with Settings

The settings file is a JSON configuration file. When modifying:
- Ensure valid JSON syntax
- Preserve existing structure when adding new settings
- Test permissions carefully before committing
- Commit changes with descriptive messages explaining what settings were changed and why
- Review permission changes to ensure security best practices
