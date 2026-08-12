# Jira Acceptance Evidence

Use this file to record evidence for the Jira story: **Build - Create the application repository template**.

## Acceptance criteria mapping

### 1. Template contains required governance files

The template contains:

- [x] `.github/workflows/` stubs
- [x] `.github/PULL_REQUEST_TEMPLATE.md`
- [x] `.github/CODEOWNERS`
- [x] `.eslintrc.json`
- [x] `.editorconfig`
- [x] `.gitignore`
- [x] `README.md`

### 2. Template prescribes no paths inside ServiceNow generated content

Confirmed by review of the repository structure.

The template does not create or reserve ServiceNow generated folders.

### 3. Marked as a GitHub template repository

Evidence to attach:

- Screenshot of GitHub repository settings showing **Template repository** enabled.

### 4. Verified additive-only

Evidence to attach:

- Screenshot or commit history showing governance files remain after the first ServiceNow generated commit.
- Confirmation that ServiceNow generated content was added without governance file conflicts.

### 5. Used to provision one test repository successfully

Evidence to attach:

- Screenshot of new repository creation using **Start with a template**.
- Link or screenshot of the successfully provisioned test repository.
- Screenshot of repository file tree after initial ServiceNow commit.

## Suggested test repository name

```text
cpa-app-test-template-validation
```

## Sign-off notes

Record outcome here:

```text
Template repository created:
Test repository provisioned:
ServiceNow initial commit completed:
Additive-only validation passed:
Reviewer:
Date:
```
