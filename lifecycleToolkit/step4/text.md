### Deploy the second version of the app

`make deploy-version-2`{{exec}}

### Checking the status of the app after making second deployment

`kubectl get pods -n podtato-kubectl`{{exec}}

### Checking the status of both the apps

`kubectl get keptnappversions -A -owide`{{exec}}