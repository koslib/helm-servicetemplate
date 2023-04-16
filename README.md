# helm-servicetemplate
Helm Service Template - tested on Python and Go apps but should work pretty much with anything.

# Usage

## Package the helm chart
`helm package ./service_template` and commit the new version into your remote chart repo. 
I use Github Pages for myself and it is hosted here: https://github.com/koslib/mycharts.

## Releases

Install a new release or upgrade:

```
helm install <release_name> <repo url> -f <path to values file>

helm upgrade <release name> <repo url> -f <path to values file>
```

Of course you can also let helm detect if release already exists otherwise install it with 

```
helm upgrade --install <release name> ...
```

# Contributions

Feel free to let me know of any feedback, open issues if you encounter any or submit your PullRequests!