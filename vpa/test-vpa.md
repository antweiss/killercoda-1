

Clone autoscaler repo
```
git clone https://github.com/kubernetes/autoscaler.git
```{{exec}}

Install vpa:
```
cd autoscaler/vertical-pod-autoscaler
./hack/vpa-up.sh
```{{exec}}

Check admission controller logs
```
kubectl logs -n kube-system -l app=vpa-admission-controller
```{{exec}}
