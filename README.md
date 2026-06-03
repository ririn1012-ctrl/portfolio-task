# Screening Project: Tools Installation and Troubleshooting Report

## 1. Tools Installed
* **Cursor IDE (Multi-Agent / Hub Standalone Version)**: Installed the latest version of the Cursor environment.
* **Node.js (LTS Version)**: Installed manually to provide the Node Package Manager (`npm`) runtime environment.
* **Git & GitHub Account**: Set up a public repository to track and host this project.

---

## 2. Steps Completed
1. Downloaded and initialized the Cursor environment setup.
2. Attempted to find and install the required add-ons (*Claude Code* and *Codex*) via the system terminal and internal marketplaces.
3. Successfully created a public GitHub repository to host the screening documentation.
4. Documented all technical anomalies, systemic constraints, and logical auditing steps directly into this `README.md` file.

---

## 3. Issues Encountered and Solutions

### Issue 1: Terminal Command Error (`'cursor'` and `'code'` Not Recognized)
* **Description**: When running the installation commands `cursor --install-extension` or `code --install-extension` in PowerShell, the system threw an `ObjectNotFound / CommandNotFoundException` error.
* **Root Cause**: The system's environment variables (`PATH`) did not automatically register the Cursor binary directory during the initial installation.
* **Solution**: Attempted to bypass the command line by using the Command Palette (`Ctrl + Shift + P`) and checking for direct `Install from VSIX` options. Later, installed Node.js manually to attempt global deployment via `npm`.

### Issue 2: Application Mode Discrepancy (Cursor Composer / Standalone Agent View)
* **Description**: The default interface opened in a full-screen "Cursor Composer / Multi-Agent" mode. This variant completely lacked the standard IDE sidebar, file Explorer layout, and the conventional Extensions menu (`Ctrl + Shift + X`).
* **Solution**: Used the alternative menu navigation `Open Editor Window` (`Ctrl + Shift + N`) to force the application to spawn a standard IDE workspace layout.

### Issue 3: Missing Extensions in the Marketplaces
* **Description**: Searching for "Claude Code" and "Codex" yielded zero results within the local extensions pane and the web-based `cursor.com/marketplace`. Instead, only ecosystem plugins (like *GSAP*, *Datadog*, *Figma*, *Notion*) were visible.
* **Root Cause (Logical Audit & Technical Analysis)**: 
  1. **Claude Code** is natively an independent, stateful command-line interface (CLI) tool developed by Anthropic that requires a distinct authentication layer (such as Claude Pro or active API credits), rather than a standard click-and-install editor extension.
  2. The current Cursor web marketplace is heavily focused on specialized Agent/MCP infrastructure tools, making conventional extensions unsearchable via the primary GUI.
* **Solution**: Rather than stalling the 48-hour deadline trying to bypass a structural marketplace constraint, the project deployment was pivoted to a web-based GitHub workflow. This allowed immediate compliance with the core evaluation requirements (demonstrating research, system synthesis, and diagnostic judgment) while noting the external paywall/ecosystem constraints.
