---
title: "Architecture"
description : "One Stop shop for hybrid cloud native application packing and deployment tools"
date: "2023-03-28"
images : []
audio : []
videos : []
series : []
tags : []
draft: false
---
[Get started]({{< relref "intro" >}})

## Architecture overview
SaaSi runs in Kubernetes and features two processing engines, the *Exporter* and the *Deployer*, to create installable *Packages*
from the *Source environment* environment and generate many *Target environment*s with customized replicas of
the exported application(s).

![](/images/saasi_arch.png)

The [SaaSi console]({{< relref "console" >}}) and the [Saasi operator]({{< relref "operator" >}}) completes the system architecture providing 
simple management interface and an orchestrated workflow.

---

Learn more on the SaaSi [Exporter]({{< relref "exporter" >}})

Learn more on the SaaSi [Deployer]({{< relref "deployer" >}})



