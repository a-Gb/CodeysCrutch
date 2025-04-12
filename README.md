# Codey's-Crutch

```
  _____          _            _            _____           _       _     
 / ____|        | |          ( )          / ____|         | |     | |    
| |     ___   __| | ___ _   _|/ ___      | |     _ __ _   | |_ ___| |__  
| |    / _ \ / _` |/ _ \ | | | / __|     | |    | '__| | | | __/ __| '_ \ 
| |___| (_) | (_| |  __/ |_| | \__ \     | |____| |  | |_| | || (__| | | |
 \_____\___/ \__,_|\___|\__, | |___/      \_____|_|   \__,_|\__\___|_| |_|
                         __/ |                                           
                        |___/                                            
```
A Docker container with modern CLI tools for development. Works on x86_64 and ARM64 architectures.

## Included Tools

### File Navigation & Search
- `fzf` - Fuzzy finder
- `ripgrep` - Fast search tool
- `fd` - Alternative to `find`
- `eza` - Modern `ls` with git integration
- `zoxide` - Smarter `cd` command
- `peco` - Interactive filtering
- `lf` - Terminal file manager
- `watchexec` - Execute on file changes

### Text Processing & Viewing
- `bat` - Cat with syntax highlighting
- `delta` - Git diff viewer
- `difftastic` - Structural diff tool
- `b3sum` - Cryptographic hash tool
- `dust` - Disk usage analyzer
- `sad` - Search and replace
- `pup` - HTML parser
- `helix` - Text editor

### Data Processing
- `jq` - JSON processor
- `yq` - YAML processor
- `jless` - JSON viewer (x86_64 only)
- `dasel` - Data structure processor
- `gron` - Make JSON greppable
- `miller` - CSV/TSV processor
- `xq` - XML processor
- `qsv` - CSV toolkit

### System & Network
- `procs` - Modern replacement for `ps`
- `doggo` - DNS client
- `xh` - HTTP client
- `gping` - Graphical ping
- `bottom` - System monitor
- `ttyd` - Terminal sharing over web
- `duf` - Disk usage utility

### Development Tools
- `hyperfine` - Benchmarking
- `tokei` - Code statistics
- `atuin` - Shell history manager
- `navi` - Interactive cheatsheet
- `nushell` - Data-aware shell
- `zellij` - Terminal workspace
- `pueue` - Task manager

### AI & NLP
- Transformers, spaCy, NLTK libraries
- OCR tools including Tesseract
- Text analysis utilities

### Other Utilities
- `pandoc` - Document converter
- `graphviz` - Graph visualization
- `imagemagick` - Image manipulation
- Text formatting tools

## Usage

```bash
./run.sh                # Start container
./run.sh --rebuild      # Rebuild image
./run.sh --restart      # Restart container
./run.sh --stop         # Stop container
./run.sh --background   # Run in background
./run.sh --web          # Web terminal (port 7681)
```

## Default Mounts
- `~/Developer/dev-codey/TEST` → `/home/dev/Developer`
- `~/Projects` → `/home/dev/Projects` (if exists)

Note: Some tools (`htmlq`, `jless`, `xsv`) available only on x86_64.
