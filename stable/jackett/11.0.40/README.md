# jackett

API Support for your favorite torrent trackers.

TrueCharts can be installed as both *normal* Helm Charts or as Apps on TrueNAS SCALE.

This readme is just an automatically generated general guide on installing our Helm Charts and Apps.
For more information, please click here: [jackett](https://truecharts.org/charts/stable/jackett)

**This chart is not maintained by the upstream project and any issues with the chart should be raised [here](https://github.com/truecharts/apps/issues/new/choose)**

## Source Code

* <https://github.com/Jackett/Jackett>

## Requirements

Kubernetes: `>=1.16.0-0`

## Dependencies

| Repository | Name | Version |
|------------|------|---------|
| https://library-charts.truecharts.org | common | 10.4.4 |

## Installing the Chart

### TrueNAS SCALE

To install this App on TrueNAS SCALE check our [Quick-Start Guide](https://truecharts.org/manual/Quick-Start%20Guides/02-Installing-an-App/).

### Helm

To install the chart with the release name `jackett`

```console
helm repo add TrueCharts https://helm.truecharts.org
helm repo update
helm install jackett TrueCharts/jackett
```

## Uninstall

### TrueNAS SCALE

**Upgrading, Rolling Back and Uninstalling the Chart**

To upgrade, rollback or delete this App from TrueNAS SCALE check our [Quick-Start Guide](https://truecharts.org/manual/Quick-Start%20Guides/04-Upgrade-rollback-delete-an-App/).

### Helm

To uninstall the `jackett` deployment

```console
helm uninstall jackett
```

## Configuration

### Helm

#### Available Settings

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.
Other values may be used from the [values.yaml](https://github.com/truecharts/library-charts/tree/main/charts/stable/common/values.yaml) from the [common library](https://github.com/k8s-at-home/library-charts/tree/main/charts/stable/common).

#### Configure using the Commandline

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`.

```console
helm install jackett \
  --set env.TZ="America/New York" \
    TrueCharts/jackett
```

#### Configure using a yaml file

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.

```console
helm install jackett TrueCharts/jackett -f values.yaml
```