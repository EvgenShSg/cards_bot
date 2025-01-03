# Virtual environment path
VENV_PATH=venv

# Default target: create and activate virtual environment, and install dependencies
install: venv install-deps

# Create virtual environment
venv:
	python3 -m venv $(VENV_PATH)

# Activate virtual environment (informational)
activate:
	@echo "To activate the virtual environment, run: source $(VENV_PATH)/bin/activate"

# Install dependencies
install-deps: venv
	$(VENV_PATH)/bin/pip install -r requirements.txt

# Clean up virtual environment
clean:
	rm -rf $(VENV_PATH)
