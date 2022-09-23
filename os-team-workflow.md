<h1>Opensource Project Workflow</h1>
<h2>Issue Workflow</h2>

* Untriaged issues are checked for validity and triaged by project managers.
* During triage:
  * Label is set to `Status: Available` if the issue is valid.
  * Label is set to `Status: On Hold` if additional information or discussion id required regarding that issue.
  * Issue is closed if it is not valid.
  * At least one label from each of `Category` and `Type` should be set.
  * Label `First Timers Only` can be set if the issue has simple fix.
  * Label `Help Wanted` can be set if the issue has a higher priority to be fixed.
* Assigning issues:
  * Contributor interested in working on a PR for the issue can comment on the issue.
  * Issues with label `Status: First Timers Only ` can be assigned to contributors who have never made a contribution to any github project.
  * 1 contributor should have only 1 assigned issue at any time.

<h2>Pull request workflow</h2>

1. When creating a Pull request for an issue, make sure all the firls of the PR template is filled in.
2. Project managers triage the PR and label `Status: Needs Review`. 
3. Request 2-3 project contributors from coding team for code review. Comment on the PR requesting code review to the @anitab-org/coding-team. 
4. Once the PR has at least 2 approvals for code review, project managers can change the label to `Status: Needs Testing`. 
5. Request at least 1-2 project contributors from the QA team for PR testing. Comment on the PR requesting code review to the @anitab-org/qa-team.
6. If the PR is high priority the label `Help Wanted`.
7. If there is a question or further discussion is needed for the PR add the label `Status: On Hold`.
8. If the testing is successful (the PR has approval fromat least 1 tester). A comment is added by the tester using the [template](https://github.com/anitab-org/mentorship-backend/blob/develop/docs/test-pr-guide.md#template-to-report-pr-testing-results).
9. The label is changed to `Status: Ready to Merge`. Contributors with Merge permissions make sure the test report looks good before merging.

<h4> Change request during code review or testing </h4>

1. Changes needed are comment by the code reviewers and the label is changed to `Status: Changes Requested`.
2. After the changes are commited the PR repeat steps 3-8 of Pull request workflow.

