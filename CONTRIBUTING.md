# Contributing Guidelines

Thank you for your interest in contributing to our projects. As a Deeptech organization, we hold our code quality to the highest standards. Please read this document carefully before submitting any code.

## 1. Development Workflow
We follow the **Gitflow** workflow.
1.  **Fork** the repository.
2.  Create a **Feature Branch** from `master` (e.g., `feat/graph-extraction-module`).
3.  Commit your changes using **Semantic Commit Messages**.
4.  Submit a **Pull Request (PR)** to the `master` branch.
5.  Wait for Code Review (at least 1 approval required).

## 2. Coding Standards
* **Style Guide:** Adhere strictly to [PEP 8](https://peps.python.org/pep-0008/).
* **Type Hinting:** All function arguments and return values must have type hints.
    * *Bad:* `def process(data):`
    * *Good:* `def process(data: Dict[str, Any]) -> List[float]:`
* **Docstrings:** All public functions and classes must have Google-style docstrings.
* **Formatters:** Run `black` and `isort` before committing.

## 3. Commit Convention
We use [Conventional Commits](https://www.conventionalcommits.org/).
* `feat`: A new feature
* `fix`: A bug fix
* `docs`: Documentation only changes
* `refactor`: A code change that neither fixes a bug nor adds a feature
* `perf`: A code change that improves performance
* `test`: Adding missing tests

**Example:** `feat(tokenizer): add support for vietnamese syllable segmentation`

## 4. Testing
* Unit tests are **mandatory** for all new features.
* Ensure all tests pass locally before pushing.
* For AI models: Include a small script to verify inference correctness.