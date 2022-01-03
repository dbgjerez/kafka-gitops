# Install Operator Lifecycle Manager (OLM)
```bash
kubectl apply -f https://raw.githubusercontent.com/operator-framework/operator-lifecycle-manager/master/deploy/upstream/quickstart/crds.yaml
kubectl apply -f https://raw.githubusercontent.com/operator-framework/operator-lifecycle-manager/master/deploy/upstream/quickstart/olm.yaml
```

Check that the operator is running
```bash
kubectl get po -n olm 
NAME                                READY   STATUS    RESTARTS   AGE
catalog-operator-6d578c5764-pgdgb   1/1     Running   0          30h
olm-operator-5b58594fc8-bjn86       1/1     Running   0          30h
operatorhubio-catalog-v57c6         1/1     Running   0          3h52m
packageserver-7cb547b686-8mtvz      1/1     Running   0          30h
packageserver-7cb547b686-tm28r      1/1     Running   0          30h

```