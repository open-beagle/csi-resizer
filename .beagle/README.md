# 说明

```bash
git remote add upstream git@github.com:kubernetes-csi/external-resizer.git
git fetch upstream
git merge v1.0.1
```

## BASEIMAGE

```bash
# x86_64
docker pull gcr.io/distroless/static:latest && \
docker tag gcr.io/distroless/static:latest registry.cn-qingdao.aliyuncs.com/wod/distroless-static:latest && \
docker push registry.cn-qingdao.aliyuncs.com/wod/distroless-static:latest

# arm64
docker pull gcr.io/distroless/static:latest-arm64 && \
docker tag gcr.io/distroless/static:latest-arm64 registry.cn-qingdao.aliyuncs.com/wod/distroless-static-arm64:latest && \
docker push registry.cn-qingdao.aliyuncs.com/wod/distroless-static-arm64:latest
```
