
<br>
In this step we will install the Lifecycle Toolkit and set up a simple app to test the app with all the tests.

## Install the Keptn Lifecycle Toolkit 

```kubectl apply -f https://github.com/keptn/lifecycle-toolkit/releases/download/v0.5.0/manifest.yaml
kubectl wait --for=condition=Available deployment/klc-controller-manager -n keptn-lifecycle-toolkit-system --timeout=120s
```{{exec}}

## Set the demo app
For the further progress of this demo, we need a sample application as well as some helpers which make it easier for your to set up your environment. These things can be found in our Getting Started repository which can be checked out as follows:

```git clone https://github.com/keptn-sandbox/lifecycle-toolkit-examples.git
cd lifecycle-toolkit-examples 
```{{exec}}

## You are done with the setting up for Lifecycle Toolkit and the demo app