# helm-servicetemplate
Helm Service Template for Python and Go apps I use

# Usage

## Package the helm chart
`helm package ./service_template` and commit the new version into https://github.com/koslibpro/mycharts.

## First time release

This command  should be executed inside the CI/CD platform, eg. Github Actions.
`helm install <release_name> <repo url> -f <path to values file>`

## Upgrade existing release

`helm upgrade <release name> <repo url> -f <path to values file>`