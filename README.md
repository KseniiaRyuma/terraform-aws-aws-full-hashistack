# Provision a Best Practices HashiStack Cluster in AWS

This Module enables Users to provision a Best Practice HashiStack Cluster in a private network with a bastion host. The end result will be a 3-Node Consul, Vault, & Nomad Cluster, with TLS/encryption setup across them. 

## Reference Material

- [Terraform Getting Started](https://www.terraform.io/intro/getting-started/install.html)
- [Terraform Docs](https://www.terraform.io/docs/index.html)
- [Consul Getting Started](https://www.consul.io/intro/getting-started/install.html)
- [Consul Docs](https://www.consul.io/docs/index.html)
- [Vault Getting Started](https://www.vaultproject.io/intro/getting-started/install.html)
- [Vault Docs](https://www.vaultproject.io/docs/index.html)
- [Nomad Getting Started](https://www.nomadproject.io/intro/getting-started/install.html)
- [Nomad Docs](https://www.nomadproject.io/docs/index.html)

## Estimated Time to Complete

5 minutes.

## Challenge

There are many different ways to provision and configure an easily accessible best practices HashiStack cluster, making it difficult to get started.

## Solution

Provision a best practices HashiStack cluster in a private network with a bastion host.

This Module provisions a 3-Node Consul, Vault, & Nomad cluster and will setup TLS/encryption across them. You can find the Packer templates to create the [Consul image](https://github.com/hashicorp/guides-configuration/blob/master/consul/consul-aws.json), [Vault image](https://github.com/hashicorp/guides-configuration/blob/master/vault/vault-aws.json), [Nomad image](https://github.com/hashicorp/guides-configuration/blob/master/nomad/nomad-aws.json) in the [Guides Configuration Repo](https://github.com/hashicorp/guides-configuration/).

## Prerequisites

- [Download Terraform](https://www.terraform.io/downloads.html)

## Steps

We will now provision the best practices HashiStack cluster.

### Step 1: Initialize

Initialize Terraform - download providers and modules.

#### CLI

[`terraform init` Command](https://www.terraform.io/docs/commands/init.html)

##### Request

```sh
$ terraform init
```

##### Response
```
```

### Step 2: Plan

Run a `terraform plan` to ensure Terraform will provision what you expect.

#### CLI

[`terraform plan` Command](https://www.terraform.io/docs/commands/plan.html)

##### Request

```sh
$ terraform plan
```

##### Response
```
```

### Step 3: Apply

Run a `terraform apply` to provision the HashiStack. One provisioned, view the `zREADME` instructions output from Terraform for next steps.

#### CLI

[`terraform apply` command](https://www.terraform.io/docs/commands/apply.html)

##### Request

```sh
$ terraform apply
```

##### Response
```
```

## Troubleshooting
To begin debugging, check the cloud-init output:

```shell
$ sudo tail -f /var/log/cloud-init-output.log
```
