# How to setup HAProxy for Redis Sentinel on Kubernetes
### Many thanks to [NSCI.IO](https://nsci.io) Data Streaming Platform, one of kind team and platform.
### Full tutorial can be found [here](https://yaniv-bhemo.medium.com/how-to-setup-haproxy-for-redis-sentinel-on-kubernetes-37ee70e44464)

### Instruction
1. helm install redis -n redis -- set sentinel.enabled=true,sentinel.quorum=2,auth.enabled=false bitnami/redis

2. choose the resolver you need in the configmap and apply haproxy.yaml


### Another tutorials:
https://www.willandskill.se/en/setup-a-highly-available-redis-cluster-with-sentinel-and-haproxy/
