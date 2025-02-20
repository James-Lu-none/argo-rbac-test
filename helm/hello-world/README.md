# Hello World

## deploy all command

```shell
argocd app create test-cloud-stage \
  --project default \
  --repo https://github.com/James-Lu-none/argo-rbac-test.git \
  --path kustomize/cloud/overlays/stage \
  --revision main \
  --dest-server https://kubernetes.default.svc \
  --dest-namespace test-cloud \
  --label argocd/appname=argoproj
```
