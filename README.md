# Python Package Template

A Cookiecutter template for Python packages with CI/CD, semantic versioning, and standard tooling.

## Features

- `pyproject.toml` configuration
- GitHub Actions CI/CD workflows
- Semantic versioning with conventional commits
- Code quality: ruff, mypy, pre-commit
- Testing: pytest
- Documentation structure

## Usage

Install Cookiecutter:

```bash
pip install cookiecutter
```

Generate a new project:

```bash
cookiecutter https://github.com/yourusername/python-package-template
```

You'll be prompted for:

- **Project name**: The name of your project
- **Package name**: Python package name (auto-generated)
- **Author name**: Your name
- **Author email**: Your email address
- **GitHub username**: Your GitHub username
- **Project description**: Brief description
- **Python version**: Minimum Python version (default: 3.9)
- **License**: License type (default: Apache-2.0)

## After generation

1. Navigate to your project directory
2. Initialise Git: `git init`
3. Add remote: `git remote add origin https://github.com/yourusername/your-project.git`
4. Install dependencies: `uv pip install -e ".[dev]"`
5. Install pre-commit hooks: `pre-commit install`

## Template Structure

```
{{cookiecutter.project_name}}/
├── src/
│   └── {{cookiecutter.package_name}}/
│       ├── __init__.py
│       └── main.py
├── examples/
│   └── quickstart.py
├── pyproject.toml
├── README.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── LICENSE
├── MANIFEST.in
└── .releaserc.json
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

Apache-2.0 License.
