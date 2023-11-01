# Use OpenAI at Azure with Python

## Prerequisites for this Example

- Windows
- One of the latest Python 3.x releases: https://www.python.org/downloads/
- Microsoft C++ Build Tools: https://visualstudio.microsoft.com/visual-cpp-build-tools/

## Run this Example

```bash
# check python version (run once)
python --version

# create new virtual environment (run once)
python -m venv .venv

# activate the virtual environment (run before each session)
.venv\Scripts\activate.ps1 # PowerShell
.venv\Scripts\activate.bat # CMD

# workaround currently necessary for Python 3.12, ignore if you use 3.11 or before (run once)
pip --require-virtualenv install aiohttp==3.9.0b0

# install openai dependency (run once)
pip --require-virtualenv install openai tenacity python-dotenv

# prepare environment variables (run once)
cp .env-template .env
code .env

# run the example script (run whenever you feel like it)
python example.py

# deactivate the virtual environment (run at the end of the session)
deactivate
```
