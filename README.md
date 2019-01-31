# Hello Kubernetes

Setup kube-ops-view:

```
helm install --name=my-release stable/kube-ops-view --namespace=kube-ops-view
```

Open kube-ops-view in your browser:

```
kubectl proxy &
open http://127.0.0.1:8001/api/v1/namespaces/kube-ops-view/services/my-release-kube-ops-view/proxy/
```
