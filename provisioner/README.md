This folder has the deployments used to deploy the nfs provisioner in fishkube.

Deployment-arm is the main deployment, configured for arm.

The test-pod had to change to an arm-compatible model

If deploying this on non-arm systems (x84_64 is easiest) just revert the test-pod.yaml top a regular busybox image and use the other eployment-arm with the contexts set.

Note: The files in `objects` have not been messed with - they are all of the individual items broken up. They were not used to directly deploy anything.