Openshift
=========

This workspace contains the basic tasks for provisioning and teardown of openshift clusters.
The layout is configured to generate an inventory file that is needed for openshift deployment.
The hooks called at the end of the provisioning call ansible to do the provisioning of openshift
based on that inventory file.

To provision Openshift in openstack you would use

```Shell
$ make openshift-on-openstack
```

The target is dependent on proper credentials and it will report if they are missing.

To destroy the openstack instance:

```Shell
$ make destroy-openshift-on-openstack
```
