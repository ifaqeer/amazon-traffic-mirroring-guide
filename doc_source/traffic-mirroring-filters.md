# Traffic mirror filters and filter rules<a name="traffic-mirroring-filters"></a>

A *traffic mirror filter* is a set of inbound and outbound traffic rules that determine the traffic that is copied from the traffic mirror source and sent to the traffic mirror destination\. By default, no traffic is mirrored\. To mirror traffic, add traffic mirror rules to the filter\. The combination of rules that you add define what traffic is mirrored\. You can also choose to mirror certain network services traffic, including Amazon DNS\. When you add network services traffic, all traffic \(inbound and outbound\) related to that network service is mirrored\.

*Traffic mirror filter rules* define what traffic is mirrored\. You define the parameters to apply to the traffic mirror source traffic to determine the traffic to mirror\. The following traffic mirror filter rule parameters are available:
+ Traffic direction \(inbound or outbound\)
+ Action \(accept or reject the packet\)
+ Protocol \(L4 protocol\)
+ Source port range
+ Destination port range
+ Source CIDR block
+ Destination CIDR block

Rules are evaluated from the lowest value to the highest value\. The first rule that matches the traffic determines the action to take\.