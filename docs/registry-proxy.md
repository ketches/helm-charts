# registry-proxy

## 使用 helm 安装

必须安装 [Helm](https://helm.sh) 才能使用 charts。请参考 [Helm 文档](https://helm.sh/docs) 开始使用。

确保 Helm 已正确设置，并且可以访问到 Kubernetes 集群。

1、添加 ketches charts 仓库

```bash
helm repo add ketches https://ketches.github.io/helm-charts
```

2、如果之前已经添加过了，那么你可能需要检索包的最新版本

```bash
helm repo update
```

3、安装 registry-proxy chart

```bash
helm install registry-proxy ketches/registry-proxy -n ketches-system --create-namespace
```

4、卸载 registry-proxy chart

```bash
helm uninstall registry-proxy -n ketches-system
```
