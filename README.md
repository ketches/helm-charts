## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:
```bash
helm repo add ketches https://ketches.github.io/helm-charts
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
ketches` to see the charts.

To install the ketches chart:
```bash
helm install ketches ketches/ketches
```
To uninstall the chart:
```bash
helm uninstall ketches
```
