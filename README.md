# godoc-bosh-release

This is a BOSH release to show documentation for private Go packages.

## Deployment Requirements
- [BOSH DNS support enabled](https://bosh.io/docs/dns/)

## Example Deployment Procedure

1. [Generate a Github API
   token](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/),
   granting it the `repo` permissions

2. Using that Github token, deploy

  ```
  bosh deploy -d godoc -n deployments/godoc.yml -l deployments/versions.yml -v github_token=<MY_GITHUB_TOKEN>
  ```
