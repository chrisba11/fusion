<!-- Code generated by gomarkdoc. DO NOT EDIT -->

# gcp

```go
import "github.com/SlalomBuild/fusion/templates/gcp"
```

Package gcp provides terraform templates for Google Cloud Platform \(GCP\)

## Index

- [Variables](<#variables>)
- [type InternalLoadBalancer](<#type-internalloadbalancer>)
  - [func NewInternalLoadBalancer(forwardingrulename, region, backendservicename, healthcheckname, networkname, subnetname string) *InternalLoadBalancer](<#func-newinternalloadbalancer>)
  - [func (resource *InternalLoadBalancer) Render(w io.Writer, skipColor bool) error](<#func-internalloadbalancer-render>)


## Variables

```go
var TEMPLATE_GCP_INTERNAL_LOADBALANCER string
```

## type [InternalLoadBalancer](<https://github.com/SlalomBuild/fusion/blob/main/templates/gcp/gcp_internal_loadbalancer.go#L16-L23>)

InternalLoadBalancer is the template data object used to create a gcp internal loadbalancer

```go
type InternalLoadBalancer struct {
    ForwardingRuleName string `help:"" default:"internal-loadbalancer"`
    Region             string `help:"" default:"us-central1"`
    BackendServiceName string `help:"" default:"backend_service"`
    HealthCheckName    string `help:"" default:"health_check"`
    NetworkName        string `help:"" default:"network"`
    SubnetName         string `help:"" default:"subnet"`
}
```

### func [NewInternalLoadBalancer](<https://github.com/SlalomBuild/fusion/blob/main/templates/gcp/gcp_internal_loadbalancer.go#L26>)

```go
func NewInternalLoadBalancer(forwardingrulename, region, backendservicename, healthcheckname, networkname, subnetname string) *InternalLoadBalancer
```

NewInternalLoadBalancer creates a new internal load balancer

### func \(\*InternalLoadBalancer\) [Render](<https://github.com/SlalomBuild/fusion/blob/main/templates/gcp/gcp_internal_loadbalancer.go#L38>)

```go
func (resource *InternalLoadBalancer) Render(w io.Writer, skipColor bool) error
```

Render generates the Terraform code for the InternalLoadBalancer



Generated by [gomarkdoc](<https://github.com/princjef/gomarkdoc>)