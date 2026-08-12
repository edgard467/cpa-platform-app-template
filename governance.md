# Repository Governance

This document summarises the governance expectations for CPA ServiceNow application repositories.

## Governance layer

The governance layer is owned and maintained by the platform team and application-owning team through GitHub.

It includes:

- Pull request template
- CODEOWNERS
- GitHub workflow stubs
- Linting configuration
- Editor configuration
- Git ignore rules
- Repository documentation

## ServiceNow generated layer

The ServiceNow generated layer is created and managed by ServiceNow source control integration.

Do not manually design or prescribe ServiceNow generated paths in this template.

Do not manually edit generated metadata unless this forms part of an approved recovery or conflict resolution process.

## Pull request governance

Pull requests should confirm:

- Linked ticket or work item
- Testing completed
- No hardcoded `sys_id` values
- Scope isolation considered
- Security-sensitive changes have appropriate review
- Deployment notes are provided where required

## Review focus areas

Reviewers should check:

- Logic correctness
- Error handling
- GlideRecord usage
- Hardcoded identifiers
- Cross-scope access
- ATF coverage
- Secrets or sensitive data
- ACL and role changes

## Branching governance

Use one branch per feature, fix, or change.

Recommended branch patterns:

```text
feature/[TICKET-ID]-short-description
bugfix/[TICKET-ID]-short-description
hotfix/[TICKET-ID]-short-description
release/vX.Y
```

Do not push directly to protected branches.

## Merge governance

Use pull requests for controlled review and merge.

Feature branches should normally merge into the active release branch.

Release branches should merge into `main` only once the relevant testing, approval, and change controls have been satisfied.
