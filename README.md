# k8s-nfs
A Kubernetes deployment of an in-cluster NFS server

``` bash
# Start an NFS server
# Importatnt: 
#    - Use the servie IP
#    - NFS path is /ova ( for example, nfs path can look like: "122.12.3.211:/pva" )
oc apply -f https://raw.githubusercontent.com/yaacov/k8s-nfs/refs/heads/main/nfs-deployment.yaml
```

```bash
# Helper http server
oc apply -f https://raw.githubusercontent.com/yaacov/k8s-nfs/refs/heads/main/ova-http-server.yaml

# curl http://ova-http-service/
```
