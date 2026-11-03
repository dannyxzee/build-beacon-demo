# Build Beacon demo pipeline

A minimal CircleCI project for testing [Build Beacon](https://zeeohn.github.io/zcodes/build-beacon/), which shows CircleCI builds and deployments on Jira issues.

1. Create a branch whose name starts with a Jira issue key from your site, e.g. `kan-1-demo` (GitHub: branch selector → type the name → Create branch).
2. CircleCI runs the `build-test-deploy` workflow on it. A branch name containing `fail` makes the test job fail.
3. Open that Jira issue: the build appears in the Development panel, and `deploy-staging` appears as a deployment once you add the rule `deploy-staging=staging` in Build Beacon's settings.
