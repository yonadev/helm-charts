# Helm charts for Yona prerequisites

This repository contains the Helm charts for the prerequisites of Yona.

To build a new version of the LDAP package:

```
helm package -d docs ldap
```

Them commit and push. The GitHub pages is configured on the /docs folder, so after the URL https://github.com/yonadev/helm-charts can be used as repository.


