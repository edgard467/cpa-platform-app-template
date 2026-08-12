# Application Repository Onboarding

Use this guide when provisioning a new ServiceNow application repository from the CPA application repository template.

## 1. Create the repository

Create a new repository in the GitHub organisation using this template.

Use the approved naming convention:

```text
cpa-app-[domain]-[function]
```

## 2. Keep the template additive-only

This template contains governance files only.

Do not add folders or files that assume the structure of the ServiceNow generated layer.

ServiceNow should create the generated application content when the scoped application is linked and committed.

## 3. Update repository metadata

Update the following files before the repository is used for application development:

- `README.md`
- `.github/CODEOWNERS`
- `.github/PULL_REQUEST_TEMPLATE.md`, if project-specific wording is needed

## 4. Apply repository controls

Apply the required GitHub repository settings for the project, including:

- Branch protection
- Pull request review requirements
- CODEOWNERS review, where required
- Secret scanning or equivalent security controls
- Required checks, when pipeline checks are available

## 5. Link the ServiceNow application

From the ServiceNow IDE or Studio source control process, link the scoped application to this repository.

Commit the initial application baseline from ServiceNow.

## 6. Validate the initial commit

After the first ServiceNow commit, confirm that:

- Governance files are still present
- ServiceNow generated content has been added by ServiceNow
- No template file forced or prescribed a ServiceNow generated path
- Pull requests can be raised successfully
- Workflow stubs do not block normal repository use
