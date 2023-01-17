# Common

This lists contains all the common keys that are used across all generators (with a few highlighted exceptions).

## Term Format

* _action::_ The action to take when matched. See Actions section for valid options.
* _comment::_ A text comment enclosed in double-quotes.  The comment can extend over multiple lines if desired, until a closing quote is encountered.
* _destination-address::_ One or more destination address tokens
* _expiration::_ Stop rendering this term after specified date in YYYY-MM-DD format. E.g. 2022-06-30
* _name::_ Name of the term.
* _option::_ See platforms supported Options section. (**Not** supported on: **k8s**, **gce**)
* _platform::_ one or more target platforms for which this term should ONLY be rendered. (**Not** supported on: **aruba**)
* _platform-exclude::_ one or more target platforms for which this term should NEVER be rendered. (**Not** supported on: **aruba**)
* _protocol::_ the network protocols this term will match, such as tcp, udp, icmp, or a numeric value.
* _source-address::_ one or more source address tokens.

<!--
build_in tokens:
            #'action',
            #'comment',
            'destination_address',
            'destination_address_exclude',
            'destination_port',
            #'expiration',
            'icmp_type',
            'stateless_reply',
            #'name',  # obj attribute, not token
            #'option',
            #'protocol',
            #'platform',
            #'platform_exclude',
            'source_address',
            'source_address_exclude',
            'source_port',
            'translated',  # obj attribute, not token
            'verbatim',
-->
