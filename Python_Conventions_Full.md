# Python Project Conventions

This document outlines the standard conventions and best practices for Python projects.

## 1. Project Structure

```
project_name/
├── src/
│   └── project_name/
│       └── __init__.py
├── tests/
│   └── test_example.py
├── docs/
├── .gitignore
├── pyproject.toml or setup.py
├── requirements.txt
├── README.md
└── CONVENTIONS.md
```

## 2. Naming Conventions

* **Packages**: lowercase, short, underscores if needed (`my_package`).
* **Modules**: lowercase (`module.py`).
* **Classes**: PascalCase (`MyClass`).
* **Functions**: snake_case (`my_function`).
* **Variables**: snake_case (`my_variable`).
* **Constants**: UPPER_CASE (`MAX_SIZE`).

## 3. Code Style

* Follow **PEP 8** wherever applicable.
* Use **4 spaces** for indentation.
* Line length should be **<= 88 characters** (recommended by Black).
* Use type hints:

```python
def process_data(data: list[str]) -> int:
    ...
```

## 4. Virtual Environments

Use a virtual environment for all development:

```
python -m venv .venv
source .venv/bin/activate  # Linux/macOS
.venv\Scripts\activate     # Windows
```

## 5. Dependency Management

* Use **requirements.txt** or **pyproject.toml**.
* Pin versions for production deployments.
* Regularly run:

```
pip install --upgrade -r requirements.txt
```

## 6. Testing

* Use **pytest** framework.
* Name test files as: `test_*.py`.
* Keep tests in `tests/` directory.
* Aim for meaningful assertions and high coverage.

## 7. Logging

* Use Python's built-in `logging` module.
* Avoid using `print()` for production-level logging.

## 8. Documentation

* Use **README.md** for project overview.
* Use **docstrings** for modules, classes, and functions.
* Prefer **Google-style** or **reST-style** docstrings.

## 9. Version Control

* Use Git with meaningful commit messages.
* Standard prefixes (optional):

  * `feat:` new feature
  * `fix:` bug fix
  * `docs:` documentation changes
  * `refactor:` non-feature code changes
  * `test:` test-related changes

## 10. Code Formatting & Tools

Recommended tools:

* **Black** for formatting
* **Flake8** or **Ruff** for linting
* **Mypy** for type checking
* **Pre-commit hooks** for automation

## 11. Packaging

* Use **pyproject.toml** with Poetry or PDM for modern packaging.
* Include meaningful metadata.

## 12. Security Considerations

* Never commit secrets; use environment variables.
* Consider `python-dotenv` or Vault for secret management.
* Keep dependencies updated.

## 13. Continuous Integration

* Use GitHub Actions or similar CI tools.
* Run tests, linting, and type checking in CI.

## 14. References

* PEP 8 – Python Style Guide: [https://peps.python.org/pep-0008/](https://peps.python.org/pep-0008/)
* Google Python Style Guide: [https://google.github.io/styleguide/pyguide.html](https://google.github.io/styleguide/pyguide.html)

---

These conventions help maintain consistency, readability, and quality across the project.
