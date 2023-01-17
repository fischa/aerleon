# PcapFilter

FILL ME IN

## Term Format

* for common keys see [common.md](common.md)

* _destination-exclude::_ Exclude one or more address tokens from the specified destination-address
* _destination-port::_ One or more service definition tokens
* _icmp-code::_ Specifies the ICMP code to filter on.
* _icmp-type::_ Specify icmp-type code to match, see section [ICMP TYPES](PolicyFormat#ICMP_TYPES.md) for list of valid arguments
* _logging::_ Specify that this packet should be logged via syslog.
* _source-exclude::_ exclude one or more address tokens from the specified source-address.
* _source-port::_ one or more service definition tokens.

## Sub Tokens

### Actions

* _accept_
* _deny_
* _next_
* _reject_

### Option

* _ack::_ Match on ACK flag being present.
* _all::_ Matches all protocols.
* _established::_ Only match established connections, implements tcp-established for tcp and sets destination port to 1024- 65535 for udp if destination port is not defined.
* _fin::_ Match on FIN flag being present.
* _is-fragment::_ Matches on if a packet is a fragment.
* _none::_ Matches none.
* _psh::_ Match on PSH flag being present.
* _rst::_ Match on RST flag being present.
* _syn::_ Match on SYN flag being present.
* _tcp-established::_ Only match established tcp connections, based on statefull match or TCP flags. Not supported for other protocols.
* _urg::_ Match on URG flag being present.
