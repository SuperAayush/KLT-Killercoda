<br>

### The Demo Application
For this demonstration, we use a slightly modified version of the PodTatoHead application.

Over time, we will evolve this application from a simple manifest to a Keptn-managed application:

We install it with kubectl then add pre- and post-deployment tasks.
For this, we check if the entry service is available before the other services are scheduled.
We then add evaluations to ensure that our infrastructure is in good shape before we deploy the application.
Finally, we evolve to a GitOps driven deployment and notify an external webhook service when the deployment has finished.


### Install the Demo Application (Version 1)
In the first version of the Demo application, the Keptn Lifecycle Toolkit evaluates metrics provided by Prometheus and checks if the specified amount of CPUs are available before deploying the application

To install it, simply apply the manifest:

`make deploy-version-1`{{exec}}