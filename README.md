# Abstractive Text Summarization with PEGASUS

An end-to-end, configurable pipeline for **abstractive text summarization** using the **PEGASUS** transformer model.  
The project includes:

- A modular training & inference pipeline (`main.py`)
- Configuration-driven experimentation (`config/`, `params.yaml`)
- A simple application entry point (`app.py`) to run the summarization service
- Supporting notebooks and research experiments (`research/`)

---

## Features

- **Abstractive Summarization with PEGASUS**  
  Uses a PEGASUS transformer model to generate human-like summaries instead of simple extractive snippets.

- **Config-Driven Pipeline**  
  All paths, hyperparameters, and pipeline options are controlled via YAML configs for easy experimentation and reproducibility.

- **Modular Components**  
  Clear separation between configuration management, data/processing components, and pipeline orchestration.

- **App Entry Point**  
  `app.py` exposes a simple interface where you can input raw text and receive a summary.

- **Research Notebooks**  
  The `research/` folder can be used for exploratory experiments, testing, and prototypes.

---

## Project Structure

```text
Abstractive_Text_Summarization_with_PEGASUS/
├─ config/
│  └─ config.yaml        # Core configuration for paths & pipeline settings
├─ research/             # Notebooks / experimentation
├─ src/
│  └─ textSummarizer/
│      ├─ ...            # Source code for data, model, and pipeline components
├─ app.py                # Application entry point (UI / API)
├─ main.py               # Orchestrates the end-to-end ML pipeline
├─ params.yaml           # Model / training hyperparameters
├─ requirements.txt      # Python dependencies
├─ Dockerfile            # Docker image definition (optional)
├─ template.py           # Utility/template script
├─ setup.py              # Package setup file
└─ README.md             # You are here 🙂
```
## Installation

1. Clone the repository
```bash
git clone https://github.com/shanuu23/Abstractive_Text_Summarization_with_PEGASUS.git
cd Abstractive_Text_Summarization_with_PEGASUS
```

2. Create and activate a virtual environment (recommended)

    A. Create a virtual environment
     ```bash
      python -m venv .venv
    ```

    B. Activate it

      a. On Linux / macOS
     ```bash
       source .venv/bin/activate
     ```

      b. On Windows (PowerShell)
     ```bash
       .venv\Scripts\Activate.ps1
     ```

3. Install dependencies
    ```bash
      pip install -r requirements.txt
    ```

4. Run the Web/App Interface

   a. Remove any stale artifacts
    ```bash
    rm -rf artifacts
    ```
    
   b. Run the app
    ```bash
    python app.py
    ```
