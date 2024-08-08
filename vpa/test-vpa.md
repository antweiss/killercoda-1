

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
