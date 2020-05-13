###nginx ingress for local dev
To start
```
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/static/provider/cloud/deploy.yaml
```

To stop
```
kubectl delete -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/static/provider/cloud/deploy.yaml
```

Verify running
```
kubectl get svc -n ingress-nginx
```

create secret if not exists
```
kubectl create secret generic pgpassword --from-literal PGPASSWORD=password
```
