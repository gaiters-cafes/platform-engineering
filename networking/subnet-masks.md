# Common subnet masks: What they represent in terms of IP addresses, and typical use cases:

| CIDR Notation | Subnet Mask         | IPs per Subnet | Usable IPs | Typical Use                             |
|---------------|----------------------|----------------|------------|-----------------------------------------|
| **/32**       | 255.255.255.255      | 1              | 1          | Single host (e.g., loopback, routing)   |
| **/31**       | 255.255.255.254      | 2              | 2          | Point-to-point links (no broadcast)     |
| **/30**       | 255.255.255.252      | 4              | 2          | Point-to-point links (small subnets)    |
| **/29**       | 255.255.255.248      | 8              | 6          | Small subnets for limited devices       |
| **/28**       | 255.255.255.240      | 16             | 14         | Small office networks or VLANs          |
| **/27**       | 255.255.255.224      | 32             | 30         | Medium-sized LANs or VLANs              |
| **/26**       | 255.255.255.192      | 64             | 62         | Medium LANs needing some expansion      |
| **/25**       | 255.255.255.128      | 128            | 126        | Larger LANs or departmental networks    |
| **/24**       | 255.255.255.0        | 256            | 254        | Standard size for most LANs or VLANs    |
| **/23**       | 255.255.254.0        | 512            | 510        | Larger LANs or inter-site connections   |
| **/22**       | 255.255.252.0        | 1,024          | 1,022      | Campus networks, multi-floor buildings  |
| **/21**       | 255.255.248.0        | 2,048          | 2,046      | Very large subnets (ISPs, large sites)  |
| **/20**       | 255.255.240.0        | 4,096          | 4,094      | Large networks (datacenters, ISPs)      |
| **/16**       | 255.255.0.0          | 65,536         | 65,534     | Very large networks or private networks |
| **/8**        | 255.0.0.0            | 16,777,216     | 16,777,214 | Reserved for large organizations (ISPs) |

### Explanation of Key Subnets
- **/32**: Isolates a single IP, commonly for loopbacks or point-to-single-point routing.
- **/24**: The most typical LAN size, suitable for a small business or single VLAN.
- **/16**: Often used for private networks in larger organizations, with enough space for thousands of devices.
- **/8**: Assigned to large entities or ISPs; typically not seen in smaller environments.

This table can guide subnet selection based on IP requirements and network segmentation needs
