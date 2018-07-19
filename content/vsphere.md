---
title: vSphere
---

# vSphere

The `openstack` CPI can be used with [vSphere](https://azure.microsoft.com/).

 * Release: [cloudfoundry-incubator/bosh-openstack-cpi-release](https://github.com/cloudfoundry-incubator/bosh-openstack-cpi-release)
 * Issues: [GitHub Issues](https://github.com/cloudfoundry-incubator/bosh-openstack-cpi-release/issues)
 * Slack: [cloudfoundry#bosh-azure-cpi](https://cloudfoundry.slack.com/messages/bosh-azure-cpi)


## Concepts

The following table maps BOSH concepts to their vSphere-native equivalents.

| BOSH              | vSphere |
| ----------------- | --------- |
| Availability Zone |  |
| Instance          |  |
| Network Subnet    |  |
| Virtual IP        |  |
| Persistent Disk   |  |
| Disk Snapshot     |  |
| Stemcell          |  |


## Feature Support


### Network

| Network Type | Support |
| ------------ | ------- |
| Manual       | Multiple networks per instance |
| Dynamic      | Not Supported |
| VIP          | Not Supported |


### Encryption

TODO


### Miscellaneous

| Feature   | Support |
| --------- | ------- |
| Multi-CPI | Not Supported |
