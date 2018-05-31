# s3 hosting

## setup

### create secrets

`kubectl create secret generic s3-key --from-literal=AccessKey=<accessKey> --from-literal=SecretKey=<secretKey>`

### deployment
`kubectl create -f kubernetes/minio.yml`
