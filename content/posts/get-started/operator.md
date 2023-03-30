---
title: "SaaSi operator"
description : "The operator to orchestrate the SaaSi workflow"
date: "2023-03-28"
images : []
audio : []
videos : []
series : []
tags : []
draft: false
---
[Get started]({{< relref "intro" >}}) | [Architecture]({{< relref "architecture" >}})

The *SaaSi operator* is the orchestrator of the SaaSi engines.

You can install it on a single or on multiple clusters, different deployment options are allowed.

Following is an example of single cluster installation:
![](/images/single-cluster.png)


And this is an example of multi cluster installation:
![](/images/multi-cluster.png)

**TODO**

The *SaaSi operator* defines its own Kubernetes API to manage the workflow, so that the whole application can work even without the
[SaaSi console]({{< relref "console" >}}), which simplifies the integration with CI/CD pipelines:
- [SaaSiExporter](https://github.com/Cloud-Native-SaaSi/saasi-exporter/crds/SaaSiExporter.yaml) is the custom resource to define a request for the [Exporter]({{< relref "exporter" >}}) service
  - [SaaSiExportResponse](https://github.com/Cloud-Native-SaaSi/saasi-exporter/crds/SaaSiExportResponse.yaml) is the related custom resource to track the status of an export request
- [SaaSiDeployer](https://github.com/Cloud-Native-SaaSi/saasi-deployer/crds/SaaSiDeployer.yaml) is the custom resource to define a request for the [Deployer]({{< relref "deployer" >}}) service
  - [SaaSiDeployResponse](https://github.com/Cloud-Native-SaaSi/saasi-deployer/crds/SaaSiDeployResponse.yaml) is the related custom resource to track the status of a deployment request


