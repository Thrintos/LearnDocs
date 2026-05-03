# Microsoft Security Certification Study Notes

> **Disclaimer:** These notes are a personal study resource and are not officially affiliated with or endorsed by Microsoft.

A community-driven collection of study notes for Microsoft Security Certifications. Whether you're preparing for SC-900, SC-200, SC-300, AZ-500, or any other Microsoft security exam, this repository aims to be a helpful, accurate, and up-to-date reference.

## 📚 About This Repository

This repository contains personal study notes organized by certification. The goal is to make security certification preparation more accessible by sharing structured, community-reviewed notes.

## 🤝 How to Contribute

Contributions are welcome and appreciated! Whether you've spotted a typo, found an outdated section, or want to add new content, here's how you can help.

### Types of Contributions

- **Bug fixes:** correct factual errors, broken links, or outdated information
- **Content additions:** add missing topics, expand existing sections, or add new exam notes
- **Formatting improvements:** improve readability, structure, or navigation
- **Typo & grammar fixes:** small fixes are just as valuable as large ones

### Step-by-Step Guide

1. **Fork** this repository by clicking the "Fork" button at the top right of this page.

2. **Clone** your fork to your local machine:
   ```bash
   git clone https://github.com/Thrintos/LearnDocs.git
   cd LearnDocs
   ```

3. **Create a new branch** for your changes:
   ```bash
   git checkout -b fix/description-of-your-change
   ```
   Use a descriptive branch name, for example:
   - `fix/sc200-incorrect-sentinel-info`
   - `add/az500-identity-protection-notes`

4. **Make your changes** to the relevant files.

5. **Commit your changes** with a clear and descriptive commit message:
   ```bash
   git add .
   git commit -m "Fix: corrected MFA configuration steps in SC-300 notes"
   ```

6. **Push** your branch to your fork:
   ```bash
   git push origin fix/description-of-your-change
   ```

7. **Open a Pull Request (PR)** on the original repository. Go to the original repo on GitHub, click **"Compare & pull request"**, fill in the PR template, and submit.

## 📝 Pull Request Guidelines

When opening a pull request, please include the following:

- **What** did you change or add?
- **Why** is this change needed? (e.g., incorrect information, missing content)
- **Source** (if applicable): a link to official Microsoft documentation or Learn modules that supports your change

Example PR description:
```
## What changed?
Updated the Conditional Access section in SC-300 notes.

## Why?
The previous notes described the legacy portal UI. Microsoft has since moved Conditional Access to the Entra admin center.

## Source
https://learn.microsoft.com/en-us/entra/identity/conditional-access/overview
```

## 📂 Repository Structure

```
/
├── docs/
│   ├── SC-900/
│   │   ├── index.md
│   │   ├── sc-900-compliance-solutions.md
│   │   ├── sc-900-glossary.md
│   │   ├── sc-900-identity-and-access.md
│   │   ├── sc-900-practice-questions.md
│   │   ├── sc-900-security-concepts.md
│   │   └── sc-900-security-solutions.md
```

Each certification folder inside `docs/` contains Markdown files organized by exam domain or topic.

## ✅ Contribution Standards

To keep the notes consistent and high-quality, please follow these guidelines:

- Write in **clear, concise English**
- Use **Markdown formatting** consistently
- Link to **official Microsoft documentation** where possible (e.g., [Microsoft Learn](https://learn.microsoft.com))
- Do **not** copy-paste content directly from Microsoft's copyrighted materials; paraphrase and summarize instead
- Keep notes **exam-objective aligned** where possible

## 🐛 Reporting Issues

If you find a mistake but don't want to submit a PR yourself, you can open an **Issue**. Just click the Issues tab at the top of this page, hit **New issue**, and describe the problem clearly. Include the file name, the section, and what you think is incorrect or missing.

## 📜 License

This project is open for community contributions. Please be mindful of Microsoft's intellectual property and do not reproduce exam questions or copy proprietary content.

## 🙏 Acknowledgements

Thanks to everyone who has contributed to improving these notes. Your input helps the entire community study smarter.

*These notes are a personal study resource and are not officially affiliated with or endorsed by Microsoft.*