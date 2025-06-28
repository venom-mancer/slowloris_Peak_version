# Slowloris Setup Guide

## Prerequisites
- Python 3.7 or higher
- pip (usually comes with Python)

## Quick Setup

### Windows (PowerShell)
```powershell
# Create virtual environment
python -m venv venv

# Activate virtual environment
.\venv\Scripts\Activate.ps1

# Install dependencies
pip install -r requirements.txt

# Install the package in development mode
pip install -e .
```

### Windows (Command Prompt)
```cmd
# Create virtual environment
python -m venv venv

# Activate virtual environment
venv\Scripts\activate.bat

# Install dependencies
pip install -r requirements.txt

# Install the package in development mode
pip install -e .
```

### Linux/macOS
```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Install the package in development mode
pip install -e .
```

## Quick Activation Scripts

### Windows
- **PowerShell**: Run `.\activate_env.ps1`
- **Command Prompt**: Run `activate_env.bat`

## Usage

After activating the virtual environment:

```bash
# Show help
python slowloris.py --help

# Basic usage (replace example.com with your target)
python slowloris.py example.com

# With more options
python slowloris.py example.com -p 80 -s 200 --https -v
```

## Dependencies

- **PySocks**: For SOCKS5 proxy support (optional, only needed with `--useproxy` flag)
- **Built-in modules**: `argparse`, `logging`, `random`, `socket`, `sys`, `time`, `asyncio`, `ssl`

## Development

To install development dependencies (optional):
```bash
pip install pytest black flake8
```

## Important Notes

⚠️ **WARNING**: This tool is for educational and research purposes only. Unauthorized use against systems you do not own or have explicit permission to test is ILLEGAL and UNETHICAL.

Always use this tool responsibly and legally. 