# release-plan/actions

Reusable actions for making use of release-plan in GitHub Actions.

See [create-release-plan-setup](https://github.com/release-plan/create-release-plan-setup) for use.

## Actions 

### check-if-release

Checks out the `ref` and determines if the current commit triggers a release.

### find-release-plan-version

Finds the version of the release plan in the current root.

### prepare

Runs `release-plan prepare` for the `ref` passed. Outputs the next version 
as determined by `release-plan prepare` as well as the output text.

Also takes as an input the version of release-plan/actions to use. This is to support
orgs and repos that restrict actions to hardcoding SHAs. 

## Development

### Release

To release, create a new release on GitHub with a tag. 
