# ETABS MCP

**AI assistants that read and work with your CSI ETABS model.**

ETABS MCP is a free [Model Context Protocol](https://modelcontextprotocol.io) (MCP) server for CSI ETABS 17 and later.
Claude, Cursor, VS Code Copilot, Windsurf, Gemini, Codex and other AI assistants use it to work with the model open in
ETABS, through the ETABS API. It is one self-contained program: no plug-in inside ETABS, no .NET to install.

**Website:** https://aecomcps.com/etabs · **Download:** [latest release](https://github.com/SHMH-MCPs/etabs-mcp-releases/releases/latest)

## What it does

- **Model discovery:** summary, stories, grids, objects, properties, groups and selection
- **Build and modify:** create and edit points, frames, areas and links; materials and sections; releases, restraints, modifiers
- **Loads:** patterns, cases, combinations, mass source, and frame, area and point loads
- **Analysis and results:** run analysis, then base reactions, displacements, drifts, frame forces, modal periods and mass ratios
- **Design:** run design and read design summaries
- **Database tables:** read, bulk edit and export ETABS tables
- **QA and revisions:** model checks, snapshots and compare, reports, and import/export (e2k, Excel, Access, XML)
- **Any other ETABS API member,** through a typed generic call bound by parameter name
- **20 workflow skills,** served as MCP prompts

Changes can be previewed. Deleting, unlocking results, opening or replacing a model and overwriting files need your
confirmation. Every change is read back and reported as verified or not. Model content stays on your PC, and a read-only
mode is available.

## Install

1. Download `etabs-mcp-<version>-win-x64.zip` from the [latest release](https://github.com/SHMH-MCPs/etabs-mcp-releases/releases/latest) and unzip it to a permanent folder.
2. Run `etabs-mcp.exe --doctor`, then `etabs-mcp.exe --setup all` (or one client, for example `--setup claude-desktop`).
3. Restart your AI client, open a model in ETABS, and ask, for example, "Summarise the open ETABS model".

## Supported versions

| ETABS | Status |
|---|---|
| 23 | Live-verified (23.3.1) |
| 22 | API-checked (22.7) |
| 17–21 | Designed for, not verified |

Requires Windows x64 and a licensed CSI ETABS on the same PC. ETABS MCP loads the CSI API assembly from your ETABS
installation and does not include it. ETABS is a product of Computers and Structures, Inc.; ETABS MCP is not affiliated
with or endorsed by CSI.

This repository holds releases only.
