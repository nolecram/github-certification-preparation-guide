# GitHub Advanced Security Revision Guide

## GitHub Advanced Security Overview

- GitHub Advanced Security provides tools to enhance the security of your codebase.
- Focuses on three primary areas:
  - **Supply Chain**: Dependency management and vulnerability detection.
  - **Code**: Code scanning and secret scanning.
  - **Environments**: Secure workflows and environments.

### Key Features

1. **Code Scanning**
   - Automatically detects vulnerabilities and coding errors.
   - Supports languages like JavaScript, Python, Java, C#, and more.
   - Can integrate third-party scanning tools using the SARIF format.

2. **Secret Scanning**
   - Detects secrets like API keys and credentials in your codebase.
   - Enabled by default for public repositories.
   - Can be configured for private repositories with custom patterns and push protection.

3. **Dependency Management**
   - Uses the Dependency Graph to identify direct, indirect, and vendored dependencies.
   - Dependabot alerts and updates vulnerable dependencies automatically.

4. **Security Overview**
   - Provides a centralized view of security issues across repositories.
   - Available for private repositories with GitHub Advanced Security.

## Best Practices

- Use a **SECURITY.md** file to communicate your security policy.
- Enable **branch protection rules** to enforce security checks.
- Use **Dependabot** to keep dependencies up to date.
- Enable **push protection** to prevent secrets from being committed.

## Key Commands and Configurations

- **Enable Secret Scanning at Scale**:
  ```yaml
  paths-ignore:
    - "foo/bar/*.js"
  ```
- **Upload SARIF File for Code Scanning**:
  ```yaml
  steps:
    - name: Upload SARIF file
      uses: github/codeql-action/upload-sarif@v1
      with:
        sarif_file: results.sarif
  ```
- **Configure Dependabot**:
  ```yaml
  version: 2
  updates:
    - package-ecosystem: "npm"
      directory: "/"
      schedule:
        interval: "daily"
  ```

## Advanced Topics

- **Push Protection**: Prevent secrets from being pushed to repositories.
- **Custom CodeQL Queries**: Write and use custom queries for advanced code scanning.
- **Security Overview Dashboard**: Monitor and manage security alerts across repositories.

## Resources

- [GitHub Advanced Security Documentation](https://docs.github.com/en/code-security)
- [CodeQL Documentation](https://codeql.github.com/docs/)

## Exam Tips

- Understand the difference between **dismiss** and **delete** for code scanning alerts.
- Familiarize yourself with the GitHub Advisory Database for known vulnerabilities.
- Know how to configure **permissions** for GITHUB_TOKEN in workflows.