# Requirements Updater

A collection of scripts to automatically update library versions in a project's `requirements.txt` file.

## Contents

This folder contains the following files:

- `update_requirements.py` - Interactive script to update `requirements.txt`
- `auto_update_requirements.py` - Automated script to update `requirements.txt`
- `update_dependencies.sh` - Script for CI/CD integration
- `install.sh` - Installation script for use in other projects
- `README.md` - This file
- `README_requirements_updater.md` - Detailed documentation of the scripts

## Installation in Other Projects

To install these scripts in another project, there are two options:

### Option 1: Use the installation script

1. Copy the `requirements_updater` folder to your computer.
2. Run the installation script, specifying the target directory:

```bash
./install.sh /path/to/your/project
```

If you don’t specify a directory, the scripts will be installed in the current directory:

```bash
cd /path/to/your/project
/path/to/requirements_updater/install.sh
```

### Option 2: Manually copy the scripts

1. Copy the necessary scripts to your project:
   - For interactive use: `update_requirements.py`
   - For automated use: `auto_update_requirements.py`
   - For CI/CD integration: `update_dependencies.sh`
   - Documentation: `README_requirements_updater.md`

2. Install the required dependencies:

```bash
pip install requests packaging tqdm
```

## Quick Usage

### Interactive Update

```bash
python update_requirements.py
```

### Automatic Update

```bash
python auto_update_requirements.py -v
```

### CI/CD Integration

```bash
./update_dependencies.sh
```

## Detailed Documentation

For detailed information about each script, refer to the `README_requirements_updater.md` file.

## Requirements

- Python 3.6 or later
- pip
- Python libraries:
  - requests
  - packaging
  - tqdm (only for the interactive script)

## License

These scripts are released under the MIT license. Feel free to use, modify, and distribute them as needed.
