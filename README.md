# Blood Pressure Analysis

This repository contains interactive tools for exploring continuous blood pressure exports. The scripts rely on Tkinter-driven dialogs to load text files, preview columns, and visualise beat-to-beat statistics.

## Installation

1. Create a virtual environment (optional but recommended).
2. Install the Python dependencies:

```bash
pip install -r requirements.txt
```

Tkinter is part of the Python standard library on most platforms, but it may need separate installation on some Linux distributions.

## Usage

Two entry points are available:

- **BPV2.py** – Opens a file picker, allows you to choose the time and pressure columns, and plots the raw pressure trace using Matplotlib.

```bash
python BPV2.py
```

- **eOGo.py** – Loads a continuous blood pressure export, offers a richer preview dialog, and computes beat-level metrics (systolic, diastolic, MAP) along with optional power spectral density analysis when SciPy is available.

```bash
python eOGo.py [--help]
```

Both scripts prompt for a `.txt` export file when launched without arguments.