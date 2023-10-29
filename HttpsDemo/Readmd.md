## 示例说明

### docker build

```ps1
docker build -f "D:\dotnet-test\HttpsDemo\HttpsDemo\Dockerfile" --force-rm -t httpsdemo  --build-arg "BUILD_CONFIGURATION=Release" --label "com.microsoft.created-by=visual-studio" --label "com.microsoft.visual-studio.project-name=HttpsDemo" "D:\dotnet-test\HttpsDemo"
```

### docker tag and push

```ps1
docker tag httpsdemo reg.wbm.ink/sample/httpsdemo:1.0
```

```ps1
docker push reg.wbm.ink/sample/httpsdemo:1.0
```

### docker compose

-   [yml](./Dockerfile)
-   docker create network

```sh
docker network create https-demo-network --subnet "172.23.0.0/25" --gateway "172.23.0.1"
```
