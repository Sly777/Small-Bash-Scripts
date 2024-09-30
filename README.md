# Small Bash Actions - Utility Scripts Collection

This repository contains a collection of utility scripts designed to help with various tasks related to file management, system maintenance, and content generation. Mostly these helps me on Obsidian app but some of them are too generic to be useful for others.

## Table of Contents

- [Small Bash Actions - Utility Scripts Collection](#small-bash-actions---utility-scripts-collection)
  - [Table of Contents](#table-of-contents)
  - [Scripts](#scripts)
    - [1. update\_md\_files](#1-update_md_files)
    - [2. update\_tech\_info](#2-update_tech_info)
    - [3. update\_links](#3-update_links)
    - [4. flush-dns](#4-flush-dns)
    - [5. compare-apps-with-cask](#5-compare-apps-with-cask)
  - [Requirements](#requirements)
  - [Installation](#installation)
  - [Contributing](#contributing)
  - [License](#license)

## Scripts

### 1. update_md_files

This script updates markdown files with custom frontmatter.

**Usage:**

```bash
./update_md_files [OPTIONS]
```

**Options:**

- `--customKey=KEY`: Specify the frontmatter key (default: tags)
- `--customValue=VALUE`: Specify the value to add (default: EncyclopediaNote)
- `-h, --help`: Display help message

### 2. update_tech_info

This script generates or updates markdown files with detailed information about technologies, libraries, frameworks, etc. using the Ollama API.

**Usage:**

```bash
./update_tech_info [OPTIONS] [TOPIC]
```

**Options:**

- `--inputfolder=<path>`: Specify input/output folder
- `--all`: Update all empty .md files in the specified folder
- `--json`: Generate JSON output
- `--debug`: Enable debug mode
- `-h, --help`: Display help message

### 3. update_links

This script updates Markdown links in files.

**Usage:**

```bash
./update_links [OPTIONS]
```

**Options:**

- `--checkFile=<file>`: Specify the file to check for links
- `--debug`: Enable debug mode
- `-h, --help`: Display help message

### 4. flush-dns

This script flushes the DNS cache on macOS.

**Usage:**

```bash
./flush-dns  [OPTION]
```

**Options:**

- `-h, --help`: Display help message

### 5. compare-apps-with-cask

This script compares applications in /Applications with available Homebrew casks.

**Usage:**

```bash
./compare-apps-with-cask [OPTION]
```

**Options:**

- `-h, --help`: Display help message

## Requirements

- Bash shell
- macOS (for flush-dns and compare-apps-with-cask scripts)
- Homebrew (for compare-apps-with-cask script)
- Ollama API (for update_tech_info script)

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/utility-scripts.git
   ```

2. Navigate to the project directory:

   ```bash
   cd utility-scripts
   ```

3. Make the scripts executable:

   ```bash
   chmod +x *
   ```

4. Add the scripts to your PATH:

   ```bash
   export PRIVATE_SCRIPTS_PATH="$HOME/{Where you put this repo}/small_bash_actions"
   export PATH="$PATH:$PRIVATE_SCRIPTS_PATH"
   ```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).
