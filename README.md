# 🎯 Multiaxis Intelligence Project Analyzer

A comprehensive Python tool for analyzing software project statistics, code metrics, and generating detailed reports in multiple formats.

[![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Code Style](https://img.shields.io/badge/code%20style-clean-brightgreen.svg)](#)

## Overview

This tool provides deep analysis of software projects, generating comprehensive statistics about:

- **Code Metrics** - Lines of code, comments, blank lines
- **Language Breakdown** - Analysis by programming language
- **Directory Structure** - Module and component analysis
- **File Analysis** - Largest files, complexity estimates
- **Architecture Insights** - Modular design assessment

Originally developed to analyze the Multiaxis Intelligence manufacturing AI platform, this tool can analyze any software project.

## Features

### 📊 **Comprehensive Statistics**
- Total files, lines, and code metrics
- Language-specific breakdowns
- Code-to-comment ratios
- Project scale assessment

### 📂 **Directory Analysis**
- Module and component breakdown
- Core architecture identification
- File distribution analysis

### 📄 **File Insights**
- Largest files identification
- Complexity scoring (Python)
- File type distribution

### 📈 **Multiple Output Formats**
- **Markdown Report** - Beautiful GitHub-compatible format
- **Text Report** - Plain text for terminal viewing
- **JSON Export** - Machine-readable data for further processing

### 🏗️ **Architecture Assessment**
- Modular design analysis
- Component relationship mapping
- Development insights and recommendations

## Quick Start

### Prerequisites
- Python 3.8 or higher
- No external dependencies required (uses only standard library)

### Installation

1. **Clone or Download**
   ```bash
   git clone https://github.com/YOUR_USERNAME/multiaxis-project-analyzer.git
   cd multiaxis-project-analyzer
   ```

2. **Run the Analyzer**
   ```bash
   # Navigate to your project directory
   cd /path/to/your/project
   
   # Run the analyzer
   python /path/to/analyze_project.py
   ```

### Usage

```bash
# Basic usage - analyze current directory
python analyze_project.py

# The tool will generate:
# - project_analysis.md    (Markdown report)
# - project_analysis.txt   (Text report)  
# - project_stats.json     (JSON data)
```

## Output Examples

### Markdown Report
Beautiful GitHub-compatible report with:
- Professional formatting and tables
- Statistics badges
- Code metrics breakdown
- Architecture insights
- Development recommendations

### Text Report
Clean terminal-friendly output with:
- Organized sections
- ASCII formatting
- Easy-to-read statistics
- Summary insights

### JSON Export
Machine-readable data including:
- Complete statistics object
- Language breakdowns
- Directory analysis
- File listings with metadata

## Supported File Types

The analyzer recognizes and processes:

| Extension | Language | Analysis |
|-----------|----------|----------|
| `.py` | Python | Full analysis + complexity |
| `.html` | HTML | Lines + basic metrics |
| `.js` | JavaScript | Lines + comment detection |
| `.css` | CSS | Styling file analysis |
| `.json` | JSON | Configuration files |
| `.md` | Markdown | Documentation |
| `.txt` | Text | General text files |
| `.bat` | Batch | Script files |

## Customization

### Exclude Directories
Modify the `exclude_dirs` set in the script:
```python
self.exclude_dirs = {
    'venv', '__pycache__', '.git', 'node_modules', 
    'dist', 'build', 'your_custom_dir'
}
```

### Add File Types
Extend the `file_extensions` dictionary:
```python
self.file_extensions = {
    '.py': 'Python',
    '.go': 'Go',
    '.rs': 'Rust',
    # Add your languages here
}
```

### Complexity Scoring
Adjust Python complexity metrics in `get_file_complexity_estimate()`:
- Function definitions (weight: 2)
- Class definitions (weight: 3)
- Control structures (if, for, while, try)

## Sample Analysis Results

Based on the Multiaxis Intelligence project analysis:

```
📊 SAMPLE PROJECT METRICS
Total Files:     156
Total Lines:     23,847
Code Lines:      19,124
Python Files:    102
Core Modules:    23
Project Scale:   🏭 Large Scale Application
```

## Advanced Features

### Architecture Detection
- **Modular Design Recognition** - Identifies core module patterns
- **Component Analysis** - Breaks down by functional areas
- **Dependency Mapping** - Shows file and directory relationships

### Development Insights
- **Documentation Coverage** - Assesses comment ratios
- **Code Quality Indicators** - Identifies high-complexity files
- **Project Health Metrics** - Overall codebase assessment

### Export Capabilities
- **Multiple Formats** - Markdown, text, and JSON
- **GitHub Integration** - Ready for repository documentation
- **Continuous Integration** - JSON output for automated analysis

## Use Cases

### 📋 **Project Documentation**
- Generate comprehensive project overviews
- Create repository documentation
- Stakeholder reporting

### 🔍 **Code Review Preparation**
- Identify large or complex files
- Assess documentation coverage
- Highlight areas needing attention

### 📈 **Development Planning**
- Track project growth over time
- Identify refactoring opportunities
- Plan architecture improvements

### 🚀 **Team Onboarding**
- Help new developers understand codebase
- Provide project structure overview
- Highlight key components

## Contributing

This tool was developed for analyzing the Multiaxis Intelligence platform but is designed to be generally useful. Contributions welcome for:

- Additional language support
- Enhanced complexity metrics
- New output formats
- Architecture analysis improvements

## License

MIT License - Feel free to use and modify for your projects.

## Credits

Developed by **Michael Kaminski**, CEO of Multiaxis LLC, for analyzing the Multiaxis Intelligence AI platform architecture.

**Related Projects:**
- [Multiaxis Intelligence](https://www.multiaxisintelligence.com) - AI-powered manufacturing platform
- [Multiaxis LLC](https://www.multiaxis.llc) - Software engineering for manufacturing

---

*"Understanding your codebase is the first step to improving it."*
