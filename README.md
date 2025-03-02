# entrypoint = "main.py"
modules = ["python-3.10:v18-20230807-322e88b"]

[nix]
channel = "stable-23_05"

[env]
VIRTUAL_ENV = "$REPL_HOME/.pythonlibs"

[unitTest]
language = "python3"

[gitHubImport]
requiredFiles = [".replit", "replit.nix"]

[deployment]
run = ["python3", "main.py"]
deploymentTarget = "cloudrun"
# myCurrentage = 30
# currentYear = 2025
# execute
