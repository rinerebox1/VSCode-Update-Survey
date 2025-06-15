# VSCode Updates January - May 2025

This document consolidates the VSCode updates from January to May 2025.

## January 2025 (version 1.97)

Key highlights from the [January 2025 (version 1.97) release notes](https://code.visualstudio.com/updates/v1_97):

*   **Copilot Next Edit Suggestions (preview)**: Copilot predicts the next edit you are likely to make.
*   **Reposition Command Palette**: Drag the Command Palette and Quick Inputs to a new position.
*   **Auto accept edits**: Automatically accept edits from Copilot after a configurable timeout.
*   **Extension publisher trust**: Keep your environment secure with extension publisher trust.
*   **Compound logs**: Combine multiple logs into a single, aggregated log view.
*   **Filter output logs**: Filter the contents of the Output panel.
*   **Git blame information**: Rich git blame information and open on GitHub.
*   **Search values in debug variables**: Filter and search for specific values in debug variables.
*   **Notebook inline values**: View inline values for code cell variables in notebooks.
*   **Python no-config debug**: Quickly debug a Python script or module without setup.

## February 2025 (version 1.98)

Key highlights from the [February 2025 (version 1.98) release notes](https://code.visualstudio.com/updates/v1_98):

*   **Next Edit Suggestions (preview)**: Collapsed mode for this Copilot feature which predicts the next edit you are likely to make.
*   **Agent mode (preview)**: Copilot autonomously completes tasks, with UI and functionality improvements.
*   **Copilot Edits for notebooks**: Iterate quickly on edits for your notebooks.
*   **Copilot Vision**: Attach and interact with images in chat prompts.
*   **Code search**: More advanced codebase search in Copilot Chat using tools like text and file search.
*   **Terminal IntelliSense (preview)**: Rich completion support for your terminal, including more Fig completion specs and better inline suggestion detection.
*   **Drag & drop references**: Quickly open peek references in a new editor.
*   **Linux custom title bar**: Custom title bar support for Linux enabled by default.
*   **Unresolved diagnostics (preview)**: Prompt when committing with unresolved diagnostics.
*   **Soft-delete in source control**: Move untracked files to trash instead of deleting them.
*   **Custom instructions GA**: Use custom instructions to tailor Copilot to your needs.

## March 2025

Key highlights from the [March 2025 (version 1.99) release notes](https://code.visualstudio.com/updates/v1_99):

*   **Agent mode**:
    *   Now available in VS Code Stable (enable with `chat.agent.enabled`).
    *   Extendable with Model Context Protocol (MCP) server tools for dynamic interaction with external tools and data.
    *   Includes new built-in tools: `#fetch` for web content, `#usages` for symbol references, and a "thinking tool" for complex tasks.
*   **Code Editing**:
    *   **Next Edit Suggestions GA**: Copilot's NES feature is now generally available.
    *   **AI Edits Improvements**: Reduced distractions (like diagnostic events) while AI applies edits.
*   **Chat**:
    *   **Bring Your Own Key (BYOK) (Preview)**: Use personal API keys for providers like Azure, Anthropic, Gemini, OpenAI, etc.
    *   **Unified Chat Experience**: Seamlessly switch between Ask, Edit, and Agent modes within a single chat view.
    *   **Faster Workspace Searches**: Instant remote workspace indexing for quicker and more accurate searches with `#codebase`/`@workspace`.
*   **Notebook Editing**:
    *   **AI Notebook Editing Improvements**: Edit and agent modes now support notebooks for creating and modifying content.
    *   **New Notebook Tool**: Create new Jupyter notebooks directly from chat using `/newNotebook` or agent/edit modes.
    *   **Navigate & Undo AI Edits**: Review AI edits across cells with diff toolbars and undo changes at the notebook level.
    *   **Cell Output in Chat**: Add text, errors, and images from cell outputs directly to chat for context.

## April 2025

Key highlights from the [April 2025 (version 1.100) release notes](https://code.visualstudio.com/updates/v1_100):

*   **Chat**:
    *   **Prompt and Instructions Files**: Aligned and improved Markdown-based custom instructions (`.instructions.md`) for providing guidelines and reusable prompt files (`.prompt.md`) for standalone chat requests.
    *   **Smarter Results with Tools**:
        *   `#githubRepo` tool: Search code within any accessible GitHub repository.
        *   `#extensions` tool: Find and install Marketplace extensions.
        *   `#fetch` tool improvements: Fetches entire web page content and formats it as Markdown.
    *   **MCP Enhancements**: Added support for image output and Streamable HTTP for Model Context Protocol servers.
*   **Chat Performance**:
    *   **Faster Responses**: Conversation summary and prompt caching lead to quicker responses on repeated chat requests.
    *   **Faster Agent Mode Edits**: Utilizes OpenAI's apply patch and Anthropic’s replace string tool for quicker edits, especially in large files.
*   **Editor Experience**:
    *   **Floating Window Modes**: Floating windows now support "Compact" (minimal UI) and "Always-on-top" modes.
    *   **Staged Changes Quick Diff**: View staged changes directly in the editor gutter.
*   **Code Editing**:
    *   **Next Edit Suggestions (NES)**: Now on by default with a new model for faster, more relevant suggestions, and can suggest missing imports (JS/TS).
    *   **Generate Alt Text**: Quick fix to generate or update alt text for images in HTML and Markdown.
*   **Notebooks**:
    *   **Agent Mode Tools**: New tools to run notebook cells, get kernel state, and list/install packages.
    *   **Drag & Drop Cell Outputs**: Easily drag image and textual cell outputs to chat as context.
*   **Languages**:
    *   **CSS/HTML Browser Support**: Hovering over CSS properties or HTML elements now shows browser compatibility (Baseline).
    *   **JS/TS Expandable Hovers (Experimental)**: Show more or less type information in hovers.
*   **Python**:
    *   **Branch Coverage**: Supported in the Testing Explorer (requires `coveragepy >= 7.7`).
    *   **Python Environments Extension**: "Quick Create" command for faster virtual environment setup and new chat tools (`#pythonGetEnvironmentInfo`, `#pythonInstallPackage`).

## May 2025

Key highlights from the [May 2025 (version 1.101) release notes](https://code.visualstudio.com/updates/v1_101):

*   **MCP (Model Context Protocol) Enhancements**:
    *   **Prompt Support**: MCP servers can define reusable prompts/tasks for LLMs, accessible via slash commands (`/mcp.servername.promptname`).
    *   **Resource Support**: Attach MCP server resources as context and browse them.
    *   **Sampling (Experimental)**: Allows MCP servers to make requests back to the model.
    *   **Authentication Support**: VS Code now supports MCP servers that require authentication.
    *   **Development Mode**: Debug MCP servers with file watching and debugger integration.
    *   **Publish from Extensions**: Extensions can now publish collections of MCP servers.
*   **Chat**:
    *   **Tool Sets**: Define and use collections of related tools in chat (e.g., `#gh-news`).
    *   **UX Improvements**: More distinct user messages, visible undo for requests, navigable attachments, streamlined implicit context.
    *   **Efficient Edit Application**: Better handling of large file edits with conditional auto-save/squiggle disabling and aligned Keep/Undo keybindings.
    *   **Fix Task Configuration Errors**: Use Copilot to fix errors in `tasks.json`.
    *   **Custom Chat Modes (Preview)**: Define personalized chat modes with specific instructions and available tools.
    *   **Agent Enhancements**: Aware of task diagnostics and terminal current working directory.
    *   **Floating Window**: Dock and New Chat actions in floating chat windows.
*   **Source Control**:
    *   **Graph View File Details**: Selecting a history item in the Source Control Graph view now shows its constituent files (tree or list).
    *   **Copilot Coding Agent Integration**: Assign and track GitHub Copilot Coding Agent tasks from within VS Code (via GitHub Pull Requests extension).
    *   **History Item in Chat**: Add specific commits or PRs as context to chat.
*   **Editor Experience**:
    *   **Find As You Type**: Option to disable find-as-you-type behavior in the Find control.
*   **Notebooks**:
    *   **Agent Follow Mode**: Automatically scroll to the cell being executed by the agent.
    *   **Configure Kernel Tool**: Agent mode tool to ensure a notebook kernel is selected and ready.
*   **Python**:
    *   **Python Extension Chat Tools**: Tools for getting environment info, installing packages, and configuring environments.
    *   **Python Environments Extension**: Create projects from templates (package/script) and support for `pyenv` and `poetry`.
