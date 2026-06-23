\# 🦅 PHOENIX - Advanced AI Assistant System



\## Overview

PHOENIX is an advanced AI assistant system with complete system control, vision capabilities, and the power to create custom tools. It runs on Windows 11 with root terminal access and provides comprehensive automation capabilities.



\---



\## 📋 Prerequisites \& Setup



\### Required Software

\- \*\*Git\*\* must be installed for version control and updates

\- \*\*LmStudio\*\* - Recommended LLM: `qwen3.5-4b-claude-4.6-opus-reasoning-distilled-v2`



\---



\## 🛠️ ComfyUI Setup Instructions



\### Step-by-Step Configuration



1\. \*\*Initial Setup\*\*

&#x20;  ```bash

&#x20;  setup.bat

&#x20;  ```

&#x20;  Run this first to configure the base environment.



2\. \*\*Image Generation Setup\*\*

&#x20;  ```bash

&#x20;  s2.bat

&#x20;  ```

&#x20;  Execute this for image generation configuration.



3\. \*\*Start ComfyUI (Low VRAM Mode)\*\*

&#x20;  ```bash

&#x20;  comfylowvram.bat

&#x20;  ```

&#x20;  Start ComfyUI with optimized low VRAM settings.



\---



\## 🎨 Icon Generation via ComfyUI



\### Bulk Image Generation

\- Generate bulk icons/images using SD Turbo (512x512)

\- Returns numbered filenames (`icon\_01.png`, `icon\_02.png`, etc.)

\- No auto-analysis - use filenames manually for UI elements



\---



\## 📹 Video Tutorial



Watch the comprehensive tutorial:  

🔗 \[YouTube Link](https://youtu.be/EsMJwK3Lgvo)



\---



\## 🔧 Core Features



\### System Control

\- \*\*Root Terminal\*\* with full administrator privileges (red background)

\- Execute system commands with timeout control

\- Process monitoring and management

\- System load statistics and health checks



\### File Management

\- Read/write files with encoding detection

\- Create directories and manage file operations

\- Trash bin with 30-day retention

\- Copy, move, delete, and restore files



\### Vision Capabilities

\- Analyze images using vision (same LLM as Main)

\- Take screenshots (full screen, active window, or select area)

\- Chart analysis for TradingView-style visualizations



\---



\## 🧠 Memory Systems



\### 4-Level Memory Architecture

1\. \*\*Main Memory\*\* - General facts and preferences

2\. \*\*Firewall Memory\*\* - Security-related information

3\. \*\*Auto Storage\*\* - Temporary storage for images, notes, etc.

4\. \*\*Cascaded Memory\*\* - Deep knowledge with keywords, summaries, detailed content, and prompt cache



\### Prompt Cache

\- Stores pre-computed prompts for faster retrieval

\- Optimizes speed through cached representations



\---



\## 🐍 Python Execution



\### Interactive Mode

\- Execute Python code interactively in the Python Execution Widget

\- Safe environment with matplotlib, numpy, pandas available

\- Errors are captured and returned for fixing



\### Script Mode

\- Save Python code to files for persistent reuse

\- Run scripts in isolation when needed



\---



\## 📊 Data Analysis \& Visualization



\### Data Explorer Widget

\- Interactive tables without pandas dependency

\- Load CSV/JSON/XLSX files into the widget



\### Plotting \& Charts

\- Create plots: line, scatter, bar, histogram

\- Financial charts with candlestick or line visualization

\- TradingView chart analysis with trend indicators



\---



\## 🌐 Network Tools



\### Connection Management

\- Port scanning for open ports on hosts

\- DNS lookups and reverse lookups

\- Interactive network map visualizer showing active connections



\### Web Operations

\- Web search via DuckDuckGo (no API key required)

\- Fetch web page content (HTML stripped)

\- Download files from URLs to local paths



\---



\## 🔐 Security \& Audit Features



\### Secrets Scanner

\- Live detection of API keys, passwords, tokens in input/code

\- Automatically masks sensitive information



\### Audit Trail

\- Blockchain-light provides cryptographically signed event chain

\- Signed audit log entries for tool calls and system events



\### Role-Based Access Control (RBAC)

\- Set user roles: `reader`, `editor`, `admin`

\- Controls permissions based on assigned roles



\---



\## 📝 Prompt Management



\### Session Continuity

\- Save prompt history to files (.phx-history.json)

\- Load previous sessions for conversation restoration

\- List all saved prompt histories



\### A/B Testing

\- Compare two prompts side-by-side

\- Highlight differences between results



\---



\## 💾 Cache \& Performance



\### Tool Call Cache

\- Automatically caches tool results for faster access

\- Clear cache when needed



\### Resource Guardian

\- Set CPU/RAM limits to prevent system overload

\- Monitor resource usage and predict bottlenecks



\### Time-Series Forecasting

\- Predict CPU/RAM trends from historical data

\- Warn about potential bottlenecks before they occur



\---



\## 🧩 Plugin System



\### Custom Plugins

\- Write and load plugins that extend functionality

\- Plugins stored in `phoenix\_plugins/` directory

\- LLM-written plugins register automatically on demand



\---



\## 🔍 Code Analysis Tools



\### Static Analysis

\- Run code review tools: ruff, mypy, pylint

\- Check Python syntax before applying edits



\### Coverage Analysis

\- Show which parts of the code are covered by tests

\- Analyze test coverage for better understanding



\---



\## 📜 Log Integration



\### Real-Time Logging

\- Stream syslog/journalctl/Windows Event Log in real-time

\- View tail lines (default: 50 lines)



\---



\## ✅ Configuration Validation



\### Config File Validator

\- Validate YAML/JSON/TOML config files for syntax errors

\- Check best practices and formatting



\---



\## 🎭 Mock Server



\### HTTP Request Interception

\- Start local mock server to intercept HTTP requests

\- Default port: 8081 (configurable)



\---



\## 🔧 Self-Modification Sandbox



\### Safe Testing Environment

\- Create sandbox project copying Phoenix source files

\- Edit files inside the sandbox without affecting originals

\- Test code in restricted environment before applying changes



\### Workflow

1\. `create\_sandbox\_project()` - Copy files to sandbox

2\. `edit\_sandboxed\_file()` - Modify sandbox files safely

3\. `test\_sandboxed\_code()` - Verify with restricted builtins

4\. `show\_self\_modify\_diff()` - Review unified diff

5\. `apply\_sandbox\_to\_phoenix()` - Apply changes to originals



\---



\## 📊 Metrics \& Monitoring



\### LLM Request Metrics

\- Track tokens, latency, and cost per request

\- Monitor performance over time



\### System Load Statistics

\- Get detailed system information

\- Check process health and detect hangs

\- Auto-heal hanging processes with restart capability



\---



\## 🔬 Advanced Tools



\### Config Validation

\- Validate YAML/JSON/TOML files for syntax and best practices



\### Environment Variables

\- Get/set environment variables dynamically



\### Directory Tree Exploration

\- Explore directory structures with configurable depth

\- List only directories when needed



\---



\## 🚀 Quick Start Commands



```bash

\# Check system info

get\_system\_info()



\# List files in current directory

list\_files(directory=".")



\# Execute a command

execute\_command(command="whoami", timeout=5000)



\# Take a screenshot

take\_screenshot(capture\_mode="active\_window")



\# Analyze an image

analyze\_image(image\_path="C:/path/to/image.png", question="What is in this image?")

```



\---





\---



\## 🔗 External Resources



\### Video Tutorial

📹 \[Comprehensive Phoenix Guide](https://youtu.be/EsMJwK3Lgvo)



\---



\## 🏷️ Tags \& Keywords

`#PHOENIX #AI-Assistant #System-Control #Vision-Capabilities #Tool-Creation #Windows11 #RootTerminal #Automation`



\---



\*Last Updated: Tuesday, June 23rd, 2026 at 11:22 AM\*

