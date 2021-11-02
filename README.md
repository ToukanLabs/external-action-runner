# external-action-runner
Runs github actions triggered from external workflows

Primarily, this is used to run private build actions for free, by using a public repo rather than private. The code can be held in a private repo (which is limited to 3000 minutes), but the action can run in a public repo, where there is no limit of action minutes

Use a `repository_dispatch` trigger to receive incoming requests.

For external repositories wishing to generate triggers, it is recommended to use the [mvasigh/dispatch-action](https://github.com/mvasigh/dispatch-action) action. Sending applications will also need a [Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) with rights to run workflow actions in this repo
