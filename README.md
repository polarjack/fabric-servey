### Fabric CA Server
config for linking to postgressql

[postgresql in docker](./docker-compose.yaml)

fabric-ca-server version
```
fabric-ca-server:
 Version: 2.0.0
 Go version: go1.14.9
 OS/Arch: darwin/amd64
```

fabric-ca-client version
```
fabric-ca-client:
 Version: 2.0.0
 Go version: go1.14.9
 OS/Arch: darwin/amd64
```

[fabric-ca-server config](./fabric-ca-server-config.yaml#L161)

change following config

```yaml
db:
  type: postgres
  datasource: host=localhost port=5432 user=postgres password=postgres dbname=fabric_ca sslmode=disable
```


### Fabric Chaincode Server

[External Chaincode Service in Hyperledger Fabric](https://medium.com/blockchainexpert-blog/external-chaincode-service-in-hyperledger-fabric-60549aeaf163)

[implement hyperledger external chaincodes on k8s cluster](https://dev.to/vanitas92/how-to-implement-hyperledger-fabric-external-chaincodes-within-a-kubernetes-cluster-34de)

[hyperledger peers doc](https://hyperledger-fabric.readthedocs.io/en/release-2.3/cc_launcher.html)