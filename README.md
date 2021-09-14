# docker-ali-container

### Demo for git

#### CI

```shell
git tag -a release-v1.71.1 -m "dns/k8s-dns-node-cache:1.17.1"
git tag
git push origin release-v1.71.1
```

#### docker pull for use

```shell

docker pull registry.cn-hangzhou.aliyuncs.com/rootrl/rootrl:1.17.1

# tag
docker tag registry.cn-hangzhou.aliyuncs.com/rootrl/rootrl:1.17.1 k8s.gcr.io/dns/k8s-dns-node-cache:1.17.1

```


### Demo for google cloud shell


```shell
docker pull k8s.gcr.io/dns/k8s-dns-node-cache:1.17.1

docker tag k8s.gcr.io/dns/k8s-dns-node-cache:1.17.1 registry.cn-hangzhou.aliyuncs.com/rootrl/rootrl/dns/k8s-dns-node-cache:1.17.1

docker login --username=rootrl registry.cn-hangzhou.aliyuncs.com

docker push registry.cn-hangzhou.aliyuncs.com/rootrl/rootrl/dns/k8s-dns-node-cache:1.17.1
```