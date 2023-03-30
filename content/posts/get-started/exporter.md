---
title: "Exporter"
description : "The SaaSi service to package your customizable installer"
date: "2023-03-28"
images : []
audio : []
videos : []
series : []
tags : []
draft: true
---
[Get started]({{< relref "intro" >}}) | [Architecture]({{< relref "architecture" >}})

The *Exporter* is a Golang service to extract configurations from a live Kubernetes environment and generate a reusable, configurable installer for the [Deployer](../deployer) application.

Both the cluster configuration and the application settings can be exported and stored in the *SaaSi packages* datastore.

The *Exporter* application is based on the community project [Crane](https://konveyor.io/tools/crane/) and generates a [kustomize](https://kustomize.io/)
installable package with options to customize:
* The destination namespaces
* The relevant application parameters and secrets
* The application images (*WIP*)

Optionally, the application can be executed as a plain CLI tool. Download the latest binaries from the [latest release](https://github.com/Cloud-Native-SaaSi/saasi-exporter/releases/).