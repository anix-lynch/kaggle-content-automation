# 🎯 Kaggle Content Automation Toolkit

> Educational toolkit for automating Kaggle notebook workflows and content management

## 🎀 Features

- **Content Mirroring**: Transform GitHub projects into Kaggle-ready notebooks
- **Workflow Automation**: Streamline repetitive Kaggle tasks
- **Brand Consistency**: Maintain consistent formatting across projects
- **Progress Tracking**: Log and monitor your Kaggle activity

## 🚀 Quick Start

### Prerequisites

```bash
# Install Kaggle CLI
pipx install kaggle

# Setup API credentials
# 1. Go to https://www.kaggle.com/settings/account
# 2. Download kaggle.json
# 3. Move to ~/.kaggle/kaggle.json
# 4. Set permissions: chmod 600 ~/.kaggle/kaggle.json
```

### Installation

```bash
# Clone the repository
git clone https://github.com/anix-lynch/kaggle-content-automation.git
cd kaggle-content-automation

# Make scripts executable
chmod +x scripts/*.sh

# Run setup checker
./scripts/check_setup.sh
```

## 📚 Usage

### Mirror GitHub Project to Kaggle

```bash
# Transform a GitHub repo into a Kaggle notebook
./scripts/mirror_to_kaggle.sh https://github.com/user/data-project
```

### Content Enhancement

```bash
# Enhance existing notebook with custom branding
./scripts/enhance_notebook.sh https://www.kaggle.com/code/user/notebook
```

### Progress Tracking

```bash
# Log your Kaggle activities
./scripts/log_activity.sh mirror 'project-name' 'kaggle-url' 'github-url' 'notes'

# View activity log
cat ~/kaggle_activity.csv
```

## 🔧 Configuration

Copy `config/config.example.env` to `config/config.env` and update with your settings:

```bash
# Kaggle API (required)
KAGGLE_USERNAME=your-username
KAGGLE_KEY=your-api-key

# Optional: Customization
AUTHOR_NAME=Your Name
AUTHOR_GITHUB=your-github-username
DEFAULT_VISIBILITY=public
```

## 📁 Structure

```
kaggle-content-automation/
├── scripts/
│   ├── check_setup.sh          # System verification
│   ├── mirror_to_kaggle.sh     # GitHub → Kaggle
│   ├── enhance_notebook.sh     # Notebook customization
│   └── log_activity.sh         # Progress tracking
├── config/
│   └── config.example.env      # Configuration template
├── templates/
│   └── notebook_template.ipynb # Base notebook structure
└── docs/
    └── TROUBLESHOOTING.md      # Common issues & solutions
```

## 🎯 Educational Use Cases

- **Portfolio Building**: Showcase projects across platforms
- **Content Syndication**: Maintain presence on multiple platforms
- **Workflow Optimization**: Reduce manual, repetitive tasks
- **Brand Management**: Consistent presentation across platforms

## 🤝 Contributing

Contributions welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) first.

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

## 🙏 Acknowledgments

- Built for educational and portfolio management purposes
- Promotes best practices in data science workflows
- Encourages proper attribution and content management

---

*This toolkit is designed for educational purposes and portfolio management. Always respect platform terms of service and provide proper attribution when working with existing content.*