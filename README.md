# dapr-infrastructure

This is a simple demo of using devcontainer to implement a dapr application.

Prerequisites
- Visual Studio Code
  - Dev Containers Extensions
- Docker engine (e.g Docker Desktop)


Clone the repository to any directory and open Visual Studio Code from inside the root folder. You should be prompted to open the folder using a container. Confirm.

Follow the next steps to setup the environment and run the dapr apps.

```
# Create virtual environment
python -m venv .venv

# Activate the virtual environment
source ./.venv/bin/activate

# Install required Phython modules.
pip install -r checkout/requirements.txt
pip install -r order-processor/requirements.txt

# Run the apps
dapr run -f dapr.yaml
```