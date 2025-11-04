# release-plan/actions

Reusable actions for making use of release-plan in GitHub Actions.

See [create-release-plan-setup](https://github.com/release-plan/create-release-plan-setup) for use.

## check-if-release

Checks out the `ref` and determines if the current commit triggers a release.

## find-release-plan-version

Finds the version of the release plan in the current root.

## prepare

Runs `release-plan prepare` for the `ref` passed. Outputs the next version 
as determined by `release-plan prepare` as well as the output text.
