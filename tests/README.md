# Tests

```bash
./bin/k8sgpt auth add --backend localai --model tinyllama --baseurl http://192.168.165.59:11443/v1
kubectl apply -f tests/problematic-pod.yaml
./bin/k8sgpt analyze --explain --filter=Pod --namespace=default
```