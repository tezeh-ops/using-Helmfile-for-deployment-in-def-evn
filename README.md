# using-Helmfile-for-deployment-in-def-evn


Deploy Kubernetes Helm Charts


Status¶

March 2022 Update - The helmfile project has been moved to helmfile/helmfile from the former home roboll/helmfile. Please see roboll/helmfile#1824 for more information.

Even though Helmfile is used in production environments across multiple organizations, it is still in its early stage of development, hence versioned 0.x.

Helmfile complies to Semantic Versioning 2.0.0 in which v0.x means that there could be backward-incompatible changes for every release.

Note that we will try our best to document any backward incompatibility. And in reality, helmfile had no breaking change for a year or so.

About¶

Helmfile is a declarative spec for deploying helm charts. It lets you…

Keep a directory of chart value files and maintain changes in version control.

Apply CI/CD to configuration changes.

Periodically sync to avoid skew in environments.

To avoid upgrades for each iteration of helm, the helmfile executable delegates to helm - as a result, helm must be installed.
