---
layout: default
title: Repository Setup & Credit Taxonomy
parent: DataSquad Handbook
nav_order: 4
---

# Repository Setup & Credit Taxonomy

All DataSquad project repos live in the [`ucla-data-science-center`](https://github.com/ucla-data-science-center) GitHub organization and must be created using the **`dsc-template`**.

The template was built by Lawrence following [UC OSPO](https://ucospo.net/) guidelines. It scaffolds the required project files so every repo starts with proper credit, licensing, and contribution standards.

---

## Creating a New Repository

1. Go to [github.com/new](https://github.com/new) or click **New repository** in the `ucla-data-science-center` organization.
2. Set **Owner** to `ucla-data-science-center`.
3. Under **Start with a template**, select **`ucla-data-science-center/dsc-template`** from the dropdown.
4. Enter a descriptive **Repository name**.
5. Set visibility to **Private** unless cleared for public access.
6. Click **Create repository**.

![Select the dsc-template when creating a new repository](/assets/img/github/dsc-template-select.png)

After creating, your repo will look like this:

![Repository created from dsc-template](/assets/img/github/dsc-template-repo.png)

Do **not** remove any of the template files. They are required for UC OSPO compliance. The sections below explain how to fill each one in.

---

## Template Files

### README.md

Customize this first. Include:

- Project title and a brief description
- Setup and installation instructions
- Usage examples
- A **Contributors** section listing all team members and their roles (see [CRediT roles](#contributor-roles-credit) below)

See the [README Template Guide](https://ucospo.net/oss-resources/) from UC OSPO.

### AUTHORS

A plain-text list of everyone who contributed to the project. Include:

- Full name
- Affiliation (e.g., UCLA Library Data Science Center)
- Role or contribution type

Update this file whenever a new team member joins the project.

### CITATION.cff

A machine-readable file that tells others how to cite the project. GitHub reads this file and displays a "Cite this repository" button.

Key fields to update:

```yaml
title: "Your Project Title"
authors:
  - family-names: Doe
    given-names: Jane
    affiliation: UCLA Library Data Science Center
date-released: "2026-01-15"
```

Learn more: [Citation File Format](https://citation-file-format.github.io/)

### CONTRIBUTING.md

Describes how others can contribute to the project. The template provides a starting point. Adjust it to match the project's workflow (e.g., branch naming, review process, issue labels).

See the [Contributing Template Guide](https://ucospo.net/oss-resources/) from UC OSPO.

### LICENSE

The template includes a **BSD-3-Clause** license. Do not change the license type without consulting your supervisor.

For background on UC licensing policy, see [UCoP's guide to choosing a license](https://ucospo.net/oss-resources/).

---

## Contributor Roles (CRediT)

Use the [CRediT (Contributor Roles Taxonomy)](https://credit.niso.org/) categories to describe each person's contribution in `README.md` and `AUTHORS`. Common roles for DataSquad projects:

| Role | Description |
| :--- | :--- |
| **Conceptualization** | Defining the research question or project goals |
| **Data Curation** | Cleaning, organizing, or managing data |
| **Formal Analysis** | Statistical or computational analysis |
| **Software** | Writing code, scripts, or tools |
| **Visualization** | Creating charts, plots, or dashboards |
| **Writing** | Drafting documentation, reports, or blog posts |
| **Supervision** | Oversight and mentorship |
| **Project Administration** | Coordinating tasks and timeline |

---

## Commit and PR Guidelines

### Commits

Write clear, descriptive commit messages. Use the present tense and keep the first line short (under 72 characters).

**Format:**

```
<type>: <short summary>
```

**Common types:**

| Type | When to use |
| :--- | :--- |
| `feat` | Adding new functionality or a new file |
| `fix` | Fixing a bug or correcting an error |
| `docs` | Updating documentation, README, or comments |
| `refactor` | Restructuring code without changing behavior |
| `data` | Adding or updating datasets |
| `style` | Formatting changes (whitespace, naming, etc.) |

**Examples:**

```
feat: add clustering script for survey data
fix: correct column name in merge step
docs: update README with setup instructions
data: add cleaned census CSV
```

Avoid vague messages like `update`, `fix stuff`, or `changes`.

### Pull Requests

Do not push directly to `main`. Use feature branches and pull requests instead.

**Workflow:**

1. Create a branch from `main`:
   ```bash
   git checkout -b your-branch-name
   ```
2. Make your changes and commit them.
3. Push the branch:
   ```bash
   git push origin your-branch-name
   ```
4. Open a pull request on GitHub targeting `main`.
5. In the PR description, briefly explain:
   - What you changed
   - Why you changed it
   - Anything a reviewer should know
6. Request a review from a teammate or supervisor.
7. After approval, merge the PR and delete the branch.

**Branch naming:** Use the format `type/short-description`, matching the commit types above.

Examples:
- `feat/add-clustering-script`
- `fix/correct-merge-column`
- `docs/update-handbook-workflow`
- `data/add-census-csv`
- `refactor/clean-data-pipeline`

### First Commit

Once you've set up a new repo from the template and customized the files, push:

```bash
git add --all
git commit -m "feat: initial project setup"
git push origin main
```

---

## Checklist Before Publishing

Before archiving or making a repo public, verify:

- [ ] All contributors are listed in `AUTHORS`
- [ ] `CITATION.cff` has the correct title, authors, and date
- [ ] `README.md` includes a Contributors section with roles
- [ ] `LICENSE` file is present and unmodified
- [ ] `CONTRIBUTING.md` reflects the current workflow

For the full list of templates, tutorials, and best practices, see the [UC OSPO OSS Resources](https://ucospo.net/oss-resources/) page.
