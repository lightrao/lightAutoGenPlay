# AutogenStudio Project

## Purpose

This project is set up to utilize the `autogenstudio` framework for building and experimenting with multi-agent applications.

## Setup and Run

Follow these steps to set up the environment and run the `autogenstudio` UI:

1.  **Create a Virtual Environment:**
    ```bash
    python3 -m venv .venvAutoGen
    ```

2.  **Activate the Virtual Environment:**
    ```bash
    source .venvAutoGen/bin/activate
    # On Windows use: .venvAutoGen\Scripts\activate
    ```

3.  **Install Dependencies:**
    Install the required packages using `uv` (or `pip`):
    ```bash
    # Using uv
    uv pip install -r requirements.txt

    # Or using pip
    # pip install -r requirements.txt
    ```
    *(Note: `requirements.txt` was generated based on `autogenstudio` and `PySocks`)*

4.  **Run AutogenStudio UI:**
    Launch the web UI. The `--appdir` flag specifies the directory where AutogenStudio will store its data.
    ```bash
    autogenstudio ui --port 8081 --appdir ./myapp
    ```

For detailed commands used during the initial setup, refer to `command.md`.

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