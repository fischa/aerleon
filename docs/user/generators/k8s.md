# K8s

The K8s header designation has the following format:

```yaml
targets:
    k8s: [direction]
```

* _direction_: defines the direction, valid inputs are INGRESS and EGRESS (default:INGRESS)

## Term Format

* for common keys see [common.md](common.md)

* _destination-exclude::_ Exclude one or more address tokens from the specified destination-address
* _destination-port::_ One or more service definition tokens
* _owner::_ Owner of the term, used for organizational purposes.
* _source-exclude::_ exclude one or more address tokens from the specified source-address.

## Sub Tokens

### Actions

* _accept_
* _deny_: Only permitted for a default deny
