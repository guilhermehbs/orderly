# 🚀 Git Standard in Orderly  

## 🔹 1. Branches (Git Flow)  
- `main`: Only stable code, ready for production.  
- `develop`: Active development, where new features are tested.  
- `feature/feature-name`: For new functionalities.  
- `bugfix/bug-name`: For bug fixes.  
- `hotfix/hotfix-name`: Urgent fixes in production.  
- `release/release-version`: Preparation for new releases.  

## 🔹 2. Semantic Commits  
We follow the [Conventional Commits](https://www.conventionalcommits.org/) standard.  

### Commit Examples:  
- `feat: add login screens`  
- `fix: fix order calculation error`  
- `chore: update project dependencies`  
- `docs: improve API documentation`  
- `refactor: optimize authentication function`  

## 🔹 3. Pull Requests  
- Always create a pull request (PR) when merging into `develop` or `main`.  
- PRs should have a **clear description** of changes.  
- Use **labels** to categorize PRs (e.g., `bug`, `enhancement`, `documentation`).  
- Request at least **one review** before merging.  
- Squash and merge small commits to keep history clean.  

## 🔹 4. Commit Messages Format  
Follow this structure for clarity and consistency:  

`<type>(<scope>): <short description>`

**Types:**  
- `feat`: New feature  
- `fix`: Bug fix  
- `config`: Maintenance tasks (dependencies, configs)  
- `docs`: Documentation changes  
- `style`: Code style changes (formatting, missing semicolons)  
- `refactor`: Code restructuring without changing functionality  
- `perf`: Performance improvements  
- `test`: Adding or updating tests  
- `ci`: Changes to CI/CD workflows  

**Scope (optional):** The area of the project affected, e.g., `auth`, `database`, `api`.  

**Example:**  

- feat(auth): add JWT authentication
- fix(database): resolve deadlock issue in transactions
- docs(readme): update installation steps


## 🔹 5. Tagging Releases  
Use Git tags for versioning based on [Semantic Versioning](https://semver.org/):  

git tag -a v1.0.0 -m "First stable release" git push origin v1.0.0

- `MAJOR`: Breaking changes  
- `MINOR`: New features (backward-compatible)  
- `PATCH`: Bug fixes and improvements  

## 🔹 6. Code Review Guidelines  
- **Follow coding standards** before submitting a PR.  
- **Write meaningful commit messages** (no `fix bug` or `updated stuff`).  
- **Break large PRs into smaller ones** when possible.  
- **Add comments** to explain complex logic.  

## 🔹 7. Git pull
- **Use this form to resolve conflicts** `git pull --rebase --autostash origin <branch-name>`