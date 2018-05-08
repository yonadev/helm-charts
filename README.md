# Helm charts for Yona

This repository contains the Helm charts for Yona, including its prerequisites. The Yona packages are automatically added through [the Jenkins build](https://yonadev.ci.cloudbees.com/job/build-and-test/job/master/).

To build a new versions of the LDAP or Hazelcast packages and update the index:

```
helm package -d docs ldap
helm package -d docs hazelcast

helm repo index docs --url https://jump.ops.yona.nu/helm-charts
```

Then commit and push.

[GitHub pages](https://pages.github.com/) is configured on the ``/docs`` folder, so the URL https://yonadev.github.io/helm-charts can be used as repository. To add the repository as "yona", run ``helm repo add yona https://yonadev.github.io/helm-charts``.
