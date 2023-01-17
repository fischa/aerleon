# WindowsAdvFirewall

The Windows Advanced Firewall header designation has the following format:

```yaml
targets:
    windows_advfirewall: {out|in} {inet|inet6|mixed}
```

* _out_: Specifies that the direction of packet flow is out. (default)
* _in_: Specifies that the direction of packet flow is in.
* _inet_: specifies that the resulting filter should only render IPv4 addresses.
* _inet6_: specifies that the resulting filter should only render IPv6 addresses.

## Term Format

* for common keys see [common.md](common.md)

* _destination-exclude::_ Exclude one or more address tokens from the specified destination-address
* _destination-port::_ One or more service definition tokens
* _icmp-type::_ Specify icmp-type code to match, see section [ICMP TYPES](PolicyFormat#ICMP_TYPES.md) for list of valid arguments
* _source-exclude::_ exclude one or more address tokens from the specified source-address.
* _source-port::_ one or more service definition tokens.

## Sub Tokens

### Actions

* _accept_
* _deny_

## WindowsIPSec

The Windows IPSec header designation has the following format:

```yaml
targets:
    windows_advfirewall: [filter_name]
```

* _filter name_: defines the name of the Windows IPSec filter.

## Term Format

* _destination-exclude::_ Exclude one or more address tokens from the specified destination-address
* _destination-port::_ One or more service definition tokens
* _source-exclude::_ exclude one or more address tokens from the specified source-address.
* _source-port::_ one or more service definition tokens.

## Sub Tokens

### Actions

* _accept_
* _deny_
