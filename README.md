# s3 hosting

## setup

### create secrets

`kubectl -n storage create secret generic s3-minio-key --from-literal=AccessKey=<accessKey> --from-literal=SecretKey=<secretKey>`

### deployment

1. `kubectl create -f kubernetes/minio-pvc.yml`
1. `kubectl create -f kubernetes/minio.yml`
1. `kubectl create -f kubernetes/tech-stouffcapital-s3-ing-ssl.yml`
