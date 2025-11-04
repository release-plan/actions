# release-plan/actions

Reusable actions for making use of release-plan in GitHub Actions.

See [create-release-plan-setup](https://github.com/release-plan/create-release-plan-setup) for use.

## Actions 

### should-prepare-release

Checks out the `ref` and determines if the current commit triggers a release.
If it is a release, don't output that prepare should run. Also only run
prepare on push event or workflow dispatch if plan wasn't updated 
(don't create a release plan when we're releasing) and only run on labeled event 
if the PR has already been merged.

### find-release-plan-version

Finds the version of the release plan in the current root.

### prepare

Runs `release-plan prepare` for the `ref` passed. Outputs the next version 
as determined by `release-plan prepare` as well as the output text.

## Development

### Release

Before a major release, update the version in prepare/action.yml where it says
`ON RELEASE:`. Unfortunately, there is no good way to dynamically reference
the version of the set of actions. 
To release, create a new release on GitHub with a tag.
