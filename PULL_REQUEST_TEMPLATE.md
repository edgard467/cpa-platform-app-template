## What does this PR do?

Provide a plain English summary of the change and why it is needed.

## Linked ticket

Reference the related Jira, ServiceNow task, or change record.

```text
ACOE-XXX - link or short description
```

## Testing performed

- [ ] ATF suite executed and all tests are passing
- [ ] Manually tested on the development instance
- [ ] No hardcoded `sys_id` values introduced
- [ ] Scope isolation confirmed
- [ ] No credentials, tokens, secrets, or sensitive data committed

## ServiceNow impact

Describe the ServiceNow artefacts or functional areas affected by this change.

Examples:

- Script Include
- Business Rule
- Client Script
- Flow Designer artefact
- ACL or role configuration
- Table or field configuration
- Integration configuration

## Deployment notes

Describe any deployment considerations, post-deployment tasks, dependent changes, rollback notes, or manual checks.

## Screenshots / ATF results / evidence

Attach screenshots, test outputs, or supporting evidence where relevant.

## Reviewer checklist

- [ ] Logic appears correct for the linked ticket
- [ ] Edge cases and null handling considered
- [ ] No hardcoded `sys_id` values
- [ ] GlideRecord usage is appropriate
- [ ] Cross-scope access is intentional and declared where needed
- [ ] Security-sensitive changes have appropriate review
- [ ] PR is ready to merge
