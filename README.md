# AutogenStudio Project

## Purpose

This project is set up to utilize the `autogenstudio` framework for building and experimenting with multi-agent applications.

## Setup and Run

Follow these steps to set up the Python virtual environment, install the necessary packages, and run the `autogenstudio` UI.

1.  **Create a Python Virtual Environment:**
    This command creates an isolated Python environment named `.venvAutoGen` in the current directory. This helps manage project-specific dependencies.
    ```bash
    python3 -m venv .venvAutoGen
    ```

2.  **Activate the Virtual Environment:**
    This command activates the newly created environment. Your terminal prompt should change to indicate that the `.venvAutoGen` environment is active.
    ```bash
    # On macOS/Linux:
    source .venvAutoGen/bin/activate
    # On Windows (Command Prompt/PowerShell):
    # .venvAutoGen\Scripts\activate
    ```

3.  **Install/Upgrade `autogenstudio`:**
    This command uses `uv` (a fast Python package installer) to install or upgrade the `autogenstudio` package to the latest version.
    ```bash
    uv pip install -U autogenstudio
    ```

4.  **Install `PySocks`:**
    This installs the `PySocks` library, which is often used to enable SOCKS proxy support for network connections.
    ```bash
    uv pip install PySocks
    ```

5.  **Install `httpx` with SOCKS support:**
    This installs the `httpx` library along with its optional SOCKS dependencies, allowing HTTP requests through SOCKS proxies.
    ```bash
    uv pip install "httpx[socks]"
    ```

6.  **Freeze Dependencies (Optional but Recommended):**
    This command lists all installed packages and their versions in the current environment and saves them to `requirements.txt`. This is useful for replicating the environment later.
    ```bash
    uv pip freeze > requirements.txt
    ```
    *(Note: If you clone this project later, you can install dependencies using `uv pip install -r requirements.txt`)*

7.  **Run AutogenStudio UI:**
    This command launches the `autogenstudio` web interface.
    *   `--port 8081`: Specifies that the UI should run on port 8081.
    *   `--appdir ./myapp`: Tells AutogenStudio to store its configuration, logs, and other data in the `./myapp` directory (it will be created if it doesn't exist).
    ```bash
    autogenstudio ui --port 8081 --appdir ./myapp
    ```

For the exact sequence of commands originally used during setup, refer to `command.md`.

## Project Structure

```
.
├── .gitignore         # Specifies intentionally untracked files that Git should ignore
├── command.md         # Detailed setup commands
├── hello.py           # Example Python script (content may vary)
├── README.md          # This file
├── requirements.txt   # Project dependencies
└── .venvAutoGen/      # Python virtual environment directory (if created as per instructions)
└── myapp/             # AutogenStudio application data directory (created on first run)