
Install k3d

```
curl -s https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash
```

Spin up cluster
```
k3d cluster create test
```

Clone autoscaler repo
```
git clone https://github.com/kubernetes/autoscaler.git
```

Install vpa:
```
cd autoscaler/vertical-pod-autoscaler
./hack/vap-up.sh
```

Check admission controller logs
```
kubectl logs -n kube-system -l app=vpa-admission-controller
```
