# external-action-runner
Runs github actions triggered from external workflows

Primarily, this is used to run private build actions for free, by using a public repo rather than private. The code can be held in a private repo (which is limited to 3000 minutes), but the action can run in a public repo, where there is no limit of action minutes

Use a repository_dispatch trigger to receive incoming requests
