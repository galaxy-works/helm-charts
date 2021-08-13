# helm-charts
A repository of *packaged* Helm charts, focused around
Galaxy Pro. For source(s) of the chart(s), see
https://github.com/galaxy-works/.

To update charts in this repo, place a copy of the packaged chart into
the `charts` folder and (re)build `index.yaml` by running the following command
from this repo's root:
```
helm repo index . --url https://raw.githubusercontent.com/galaxy-works/helm-charts/master
```

To package a chart to start with, run the a command like the following from the
given chart's repo. This will place the chart into `packaged-charts` subdir.
```
helm package -d ./packaged-charts/ .
```
