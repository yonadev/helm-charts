# Helm charts for Yona prerequisites

This repository contains the Helm charts for the prerequisites of Yona.

To build a new version of the LDAP package and update the index:

```
helm package -d docs ldap
helm repo index docs --url https://yonadev.github.io/helm-charts
```

Them commit and push. The GitHub pages is configured on the /docs folder, so after the URL https://github.com/yonadev/helm-charts can be used as repository. To add the repository as "yona", run ``helm repo add yona https://yonadev.github.io/helm-charts``.
