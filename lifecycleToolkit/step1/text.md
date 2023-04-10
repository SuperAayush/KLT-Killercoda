
<br>
In this step we will install the Lifecycle Toolkit and set up a simple app to test the app with all the tests.

## Install the Keptn Lifecycle Toolkit 

```
helm repo add klt https://charts.lifecycle.keptn.sh
helm repo update
helm upgrade --install keptn klt/klt -n keptn-lifecycle-toolkit-system --create-namespace --wait
```{{exec}}

## Install Demo Application
For the further progress of this demo, we need a sample application as well as some helpers which make it easier for your to set up your environment. These things can be found in our Getting Started repository which can be checked out as follows:

```
git clone https://github.com/keptn-sandbox/lifecycle-toolkit-examples.git
cd lifecycle-toolkit-examples
```{{exec}}

## You are done with the setting up for Lifecycle Toolkit and the demo app