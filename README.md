# argocd-echoserver

Argo CDにhelm-echoserverを登録するためのApp for Appsマニフェスト。

```
$ argocd app create apps \
  --repo https://github.com/VirtualTech-DevOps/argocd-echoserver.git \
  --path manifest \
  --dest-server https://kubernetes.default.svc \
  --revision main \
  --sync-policy automated \
  --dest-namespace argocd
```
