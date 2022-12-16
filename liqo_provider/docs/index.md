---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "liqo Provider"
subcategory: ""
description: |-
  Interact with Liqo.
---

# liqo Provider

Interact with Liqo.

## Example Usage

```terraform
# Initialization of kubernetes clients
provider "liqo" {
  kubernetes = {
    config_path = "path/to/kubeconfig"
  }
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `kubernetes` (Attributes) (see [below for nested schema](#nestedatt--kubernetes))

<a id="nestedatt--kubernetes"></a>
### Nested Schema for `kubernetes`

Optional:

- `client_certificate` (String) PEM-encoded client certificate for TLS authentication.
- `client_key` (String) PEM-encoded client certificate key for TLS authentication.
- `cluster_ca_certificate` (String) PEM-encoded root certificates bundle for TLS authentication.
- `config_context` (String)
- `config_context_auth_info` (String)
- `config_context_cluster` (String)
- `config_path` (String) Path to the kube config file. Can be set with KUBE_CONFIG_PATH.
- `config_paths` (List of String)
- `exec` (Attributes) (see [below for nested schema](#nestedatt--kubernetes--exec))
- `host` (String) The hostname (in form of URI) of Kubernetes master.
- `insecure` (Boolean) Whether server should be accessed without verifying the TLS certificate.
- `password` (String) The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint.
- `proxy_url` (String) URL to the proxy to be used for all API requests
- `token` (String) Token to authenticate an service account
- `username` (String) The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint.

<a id="nestedatt--kubernetes--exec"></a>
### Nested Schema for `kubernetes.exec`

Required:

- `api_version` (String)
- `command` (String)

Optional:

- `args` (List of String)
- `env` (Map of String)