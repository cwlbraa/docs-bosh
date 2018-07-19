---
title: Microsoft Azure
---

# Microsoft Azure

The `azure` CPI can be used with [Microsoft Azure](https://azure.microsoft.com/).

 * Release: [cloudfoundry-incubator/bosh-azure-cpi-release](https://github.com/cloudfoundry-incubator/bosh-azure-cpi-release)
 * Issues: [GitHub Issues](https://github.com/cloudfoundry-incubator/bosh-azure-cpi-release/issues)
 * Slack: [cloudfoundry#bosh-azure-cpi](https://cloudfoundry.slack.com/messages/bosh-azure-cpi)


## Concepts

The following table maps BOSH concepts to their Azure-native equivalents.

| BOSH              | Microsoft Azure |
| ----------------- | --------------- |
| Availability Zone |  |
| Instance          |  |
| Network Subnet    |  |
| Virtual IP        | Reserved IP |
| Persistent Disk   |  |
| Disk Snapshot     |  |
| Stemcell          |  |


## Feature Support


### Network

| Network Type | Support |
| ------------ | ------- |
| Manual       | Multiple networks per instance |
| Dynamic      | Multiple networks per instance |
| VIP          | Single network per instance |


### Encryption

AWS supports encryption functionality through their [Key Management Service](https://aws.amazon.com/kms/) using both IaaS-managed or customer-managed keys. The `encrypted` and `kms_key_arn` cloud properties for disks can be used to configure encryption settings.

**Managed Disks** - encryption is automatically used by all disks and cannot be disabled. With Managed Disks, all aspects of the encryption are managed behind the scenes of Azure.

**Storage Accounts** -
#### Managed Disks

| Disk Type       | Support |
| --------------- | ------- |
| Root Disk       | Required, cannot be disabled |
| Ephemeral Disk  | Required, cannot be disabled |
| Persistent Disk | Implicit, cannot be disabled |


#### Storage Accounts

| Disk Type       | Support |
| --------------- | ------- |
| Root Disk       | Required |
| Ephemeral Disk  |  |
| Persistent Disk |  |




### Miscellaneous

| Feature   | Support |
| --------- | ------- |
| Multi-CPI | Not Supported |
