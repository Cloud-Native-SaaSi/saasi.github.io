---
title: "SaaSi console"
description : "The SaaSi console for SaaSi operations"
date: "2023-03-28"
images : []
audio : []
videos : []
series : []
tags : []
draft: false
---
[Get started]({{< relref "intro" >}}) | [Architecture]({{< relref "architecture" >}})

The *SaaSi console* is an optional component that can be installed to provide visual access to the operations for the managed users:

The *exporter* (e.g. the SRE of the software provider) can access the *Exporter* view to manage installable packages:

{{< figure src="/images/exporter-view.png" caption="Figure 1: Exporter view" >}}

The *deployer* can access the *Deployer* view to manage client environments:

{{< figure src="/images/deployer-view.png" caption="Figure 2: Deployer view" >}}

The *admin* takes care of configuring and managing *SaaSi* for what concerns all the system-related aspects (users, performance, troubleshooting)

{{< figure src="/images/admin-view.png" caption="Figure 3: Admin view" >}}

The console is designed as a containerized application and connects the *SaaSi operator* for all the managed operations.

**TODO**

The *SaaSi console* is designed as a Node.js [backend](https://github.com/Cloud-Native-SaaSi/saasi-console-backend) feeding the console
[frontend](https://github.com/Cloud-Native-SaaSi/saasi-console-frontend), which is based on the [PatternFly](https://www.patternfly.org/v4/) design system
to make it consistent with the styles and patterns adopted by [Red Hat OpenShift](https://docs.openshift.com/container-platform/4.12/web_console/dynamic-plug-in/dynamic-plug-in.html)

