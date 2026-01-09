## Getting Started

### Running on Google Colab (easiest)

The easiest way to run the notebooks is via Google Colab, which provides free access to GPU:

1. Click the "Open in Colab" button next to any notebook above
2. To enable GPU: **Runtime** → **Change runtime type** → select **T4 GPU** → **Save**

### Running Locally

**Option 1: Using uv (Recommended)**

[uv](https://docs.astral.sh/uv/) is a fast Python package installer and resolver:

```bash
# Install uv if you don't have it
curl -LsSf https://astral.sh/uv/install.sh | sh

# Create and activate a virtual environment
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
uv pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

**Option 2: Using venv and pip**

```bash
# Create a virtual environment
python -m venv .venv

# Activate it
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```