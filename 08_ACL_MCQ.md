# ACL (Access Control List) MCQ Quiz

---

## EASY LEVEL

### Q1: What is an ACL?
A) List of rules allowing/denying traffic
B) Defines security policy
C) Applied to interfaces for filtering
D) All of above

**Answer: D**

---

### Q2: Two main ACL types:
A) Standard and Extended
B) Inbound and Outbound
C) Static and Dynamic
D) IPv4 and IPv6

**Answer: A**

---

### Q3: Standard ACL can filter on:
A) Source IP only
B) Destination IP
C) Port numbers
D) Protocols

**Answer: A**

---

### Q4: Extended ACL can filter on:
A) Source and destination IP
B) Protocol and port numbers
C) Both A and B
D) Everything

**Answer: C**

---

### Q5: ACL number for standard IPv4:
A) 1-99
B) 1-199
C) 100-199
D) No standard

**Answer: A**

---

### Q6: ACL number for extended IPv4:
A) 1-99
B) 100-199
C) 1000-1099
D) Any above 100

**Answer: B**

---

### Q7: Create standard ACL:
A) `access-list 1 permit 192.168.1.0 0.0.0.255`
B) `permit 192.168.1.0 0.0.0.255`
C) `acl 1 permit`
D) `create acl 1`

**Answer: A**

---

### Q8: Create extended ACL:
A) `access-list 101 permit tcp 192.168.1.0 0.0.0.255 any eq 80`
B) Must specify protocol, source, destination, port
C) Both true
D) `create extended-acl`

**Answer: C**

---

### Q9: Apply ACL to interface:
A) `access-group 1 in/out` (at interface)
B) `ip access-group 1 in`
C) Both syntaxes valid
D) `apply-acl 1`

**Answer: C**

---

### Q10: ACL direction - what does "in" mean?
A) Traffic entering interface
B) Traffic coming from interface
C) Both same direction
D) Depends on context

**Answer: A**

---

### Q11: Wildcard mask in ACL:
A) Same as subnet mask
B) Inverted subnet mask (1=match, 0=ignore)
C) Both true
D) Different concept

**Answer: B**

---

### Q12: Implicit deny at end of ACL:
A) Traffic not matching any rule allowed by default
B) All traffic not matching rules denied
C) Explicit deny needed
D) No implicit behavior

**Answer: B**

---

### Q13: View ACL configuration:
A) `show access-lists`
B) `show ip access-lists`
C) Both show ACLs
D) `show acl`

**Answer: C**

---

### Q14: Delete ACL line:
A) `no access-list 1`
B) Must remove entire ACL then recreate
C) `no 10` (line number)
D) Individual line deletion not possible

**Answer: B**

---

### Q15: Permit specific IP traffic:
A) `access-list 1 permit 192.168.1.1`
B) Any source to any destination?
C) Source only in standard ACL
D) Both A and C

**Answer: D**

---

### Q16: Named ACL (modern):
A) `ip access-list standard Sales`
B) `permit 192.168.1.0 0.0.0.255`
C) Both sequences
D) Subnet masks provide names

**Answer: C**

---

### Q17: Deny vs Permit in ACL:
A) Permit = allow, Deny = block
B) Order matters (first match wins)
C) Both true
D) Deny always checked first

**Answer: C**

---

### Q18: ACL on router vs switch:
A) Router filters routed traffic
B) VLAN ACL filters bridged traffic
C) Both filtering contexts
D) Same ACL applies everywhere

**Answer: C**

---

### Q19: ACL statistics (matches):
A) `show access-lists` displays count
B) Useful for troubleshooting
C) Both true
D) No statistics available

**Answer: C**

---

### Q20: Log ACL matches:
A) `log` parameter at end of rule
B) `log-input` shows source interface
C) Both logging options
D) No logging capability

**Answer: C**

---

## MEDIUM LEVEL

### Q21: Configure extended ACL permit HTTPS (port 443) from 10.0.0.0/24 to any:
A) `access-list 101 permit tcp 10.0.0.0 0.0.0.255 any eq 443`
B) Destination is "any" - implicit
C) Both correct
D) `eq` means equals/port

**Answer: A**

---

### Q22: Deny Telnet (port 23), permit all else:
A) `access-list 101 deny tcp any any eq 23`
B) `access-list 101 permit ip any any`
C) Both required in order
D) Only deny needed

**Answer: C**

---

### Q23: ACL for specific network range:
A) Wildcard mask defines range
B) Host route = 0.0.0.0 wildcard (/32)
C) Both concepts
D) Range not in ACL

**Answer: C**

---

### Q24: Remove ACL from interface (keep ACL):
A) `no ip access-group 101 in`
B) `remove acl 101`
C) At interface level: A is correct
D) `delete access-group`

**Answer: A**

---

### Q25: Inbound ACL performance (vs outbound):
A) Checked before routing
B) Denied traffic never routed
C) Both advantages
D) Same performance

**Answer: C**

---

### Q26: Permit traffic from network, deny specific host:
A) Order specific (deny) first, then permit network
B) `access-list 101 deny ip 192.168.1.1 host`
C) Both sequencing
D) Any order fine

**Answer: C**

---

### Q27: ACL for DNS (port 53):
A) Can use protocol `dns` or port `eq 53`
B) Both TCP and UDP possible
C) Both protocols typically needed
D) TCP only

**Answer: C**

---

### Q28: Configure RoCE (Remote Direct Memory Access) filtering:
A) Port 4791/4792
B) Custom ACL with specific ports
C) Both practices
D) No ACL for RoCE

**Answer: C**

---

### Q29: ACL for ICMP (ping):
A) `access-list 101 permit icmp any any`
B) ICMP is protocol, not TCP/UDP
C) Both true
D) `protocol 1` for ICMP

**Answer: B**

---

### Q30: Port range in ACL:
A) `range 80 443` for ports 80-443
B) `eq 80` for specific
C) Both operators available
D) `between` syntax also available

**Answer: D**

---

### Q31: Source port filtering:
A) `source-port` keyword
B) Less common than destination
C) Both true
D) Not possible

**Answer: B**

---

### Q32: ACL to permit established connections only:
A) `established` keyword for TCP
B) Only responses to initiated connections
C) Both true
D) Not possible

**Answer: C**

---

### Q33: Named extended ACL with permit/deny:
A) `ip access-list extended FILTER`
B) `permit tcp ... eq 443`
C) Modern and clearer syntax
D) All true

**Answer: D**

---

### Q34: ACL with traffic logging:
A) `permit tcp ... eq 443 log`
B) Syslog message generated per match
C) Both consequences
D) `logging` command separate

**Answer: C**

---

### Q35: Modify line in named ACL:
A) Add/insert new rules
B) Delete specific line number
C) Both possible in named ACL
D) Can't modify

**Answer: C**

---

### Q36: ACL for GRE (protocol 47):
A) `permit 47 source dest`
B) Used for tunnels
C) Both true
D) `protocol gre`

**Answer: C**

---

### Q37: Any/any wildcard:
A) `any` matches all addresses
B) Equivalent to `0.0.0.0 255.255.255.255`
C) Both true
D) Different meaning

**Answer: C**

---

### Q38: ACL to deny specific subnet, permit network:
A) More specific (deny) rule placed first
B) Order matters - first match wins
C) Both true
D) No specific order required

**Answer: C**

---

### Q39: Special IP addresses in ACL:
A) `host` = /32
B) `any` = 0.0.0.0/0
C) Both keywords useful
D) Always use CIDR

**Answer: C**

---

### Q40: Ephemeral port range filtering:
A) Typically 1024-65535 source ports
B) Dynamic ports for client connections
C) Both characteristics
D) Not typically filtered

**Answer: C**

---

## HARD LEVEL

### Q41: Design ACL for DMZ segmentation:
A) Permit only specific ports inbound
B) Deny internet-to-inside traffic
C) Both security layers
D) VLANs sufficient alone

**Answer: C**

---

### Q42: Implement reflexive ACL (stateful filtering):
A) `permit tcp any any eq 80 reflect RULES`
B) `permit tcp any any eq 80 established`
C) Both mechanisms track state
D) ACLs stateless inherently

**Answer: C**

---

### Q43: ACL with DSCP/QoS marking:
A) ACL identifies traffic type
B) Mark for QoS treatment
C) Both in pipeline
D) ACL doesn't mark

**Answer: C**

---

### Q44: Implement ACL for private address blocking:
A) Deny 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16
B) Permit legitimate traffic only
C) Both filtering principles
D) No need to filter private

**Answer: C**

---

### Q45: Design ACL for data exfiltration prevention:
A) Monitor outbound traffic to unknown destinations
B) Restrict file transfer protocols
C) Both prevention measures
D) ACL insufficient alone

**Answer: C**

---

### Q46: ACL in hub-and-spoke WAN topology:
A) Filters traffic at core
B) Spoke-to-spoke traffic controlled
C) Both filtering points
D) Only at spokes

**Answer: C**

---

### Q47: Implement ACL for DPI (Deep Packet Inspection):
A) ACL identifies application layer traffic
B) More sophisticated than standard port filtering
C) Both concepts
D) ACL not for DPI

**Answer: C**

---

### Q48: ACL for rate limiting (QoS class):
A) ACL identifies traffic category
B) QoS policy applies limiting
C) Both needed together
D) ACL does rate limiting

**Answer: C**

---

### Q49: Design ACL for wireless network:
A) WLAN security BEFORE ACL
B) MAC-based filtering in addition
C) Both layers
D) ACL sufficient alone

**Answer: C**

---

### Q50: ACL with BGP route filtering:
A) Filters routes advertised
B) Input/output route-maps with ACL
C) Both concepts
D) ACL not for BGP

**Answer: C**

---

### Q51: Implement ACL for compliance (PCI-DSS):
A) Restrict sensitive data access
B) Audit logging enabled
C) Both compliance measures
D) No ACL compliance needed

**Answer: C**

---

### Q52: Design ACL for cloud connectivity:
A) VPN traffic permitted specifically
B) Non-VPN blocked to cloud resources
C) Both filtering rules
D) All cloud traffic open

**Answer: C**

---

### Q53: ACL with IPv6 support:
A) `ipv6 access-list` separate from IPv4
B) Rules for IPv6 addresses need separate list
C) Both true
D) Same ACL for both

**Answer: C**

---

### Q54: Implement ACL with NAT interaction:
A) ACL checked before/after NAT translation (context-dependent)
B) Route map may include ACL
C) Both considerations
D) No interaction

**Answer: C**

---

### Q55: Design ACL for botnet/malware blocking:
A) Known malicious IP ranges denied
B) Threat intelligence integrated
C) Both prevention strategies
D) Not feasible with ACL

**Answer: C**

---

### Q56: ACL for inter-VLAN routing:
A) SVI interfaces have ACLs applied
B) Controls traffic between VLANs
C) Both routing controls
D) VLANs don't use ACLs

**Answer: C**

---

### Q57: Implement VACL (VLAN ACL) on switch:
A) Applies within/between VLANs
B) Different ACL system than routers
C) Both characteristics
D) Same as routing ACL

**Answer: C**

---

### Q58: Design ACL for network segmentation (zero-trust):
A) Deny all by default
B) Permit only required flows
C) Both principles
D) Default permit model

**Answer: C**

---

### Q59: ACL for high-performance filtering (hardware):
A) Context-dependent (switches faster)
B) Router ACL slower if extensive
C) Both performance considerations
D) Always same speed

**Answer: C**

---

### Q60: Implement ACL for test traffic isolation:
A) Test VLANs with specific ACL rules
B) Production traffic untouched
C) Both segregation methods
D) No special handling

**Answer: C**

---

### Q61: Design ACL with permit and deny logging:
A) Both `log` enabled for dual visibility
B) Identify blocked vs allowed traffic
C) Both true
D) One direction use only

**Answer: C**

---

### Q62: ACL for network reconnaissance prevention:
A) Block unusual port scans
B) NMAP fingerprinting detection
C) Both reconnaissance types
D) Not detectable via ACL

**Answer: C**

---

### Q63: Implement ACL for backup network:
A) Specific backup server IP/port
B) Limit backup traffic
C) Both control measures
D) No restricting backup

**Answer: C**

---

### Q64: Design ACL with policy-based routing:
A) Route-map with ACL match criteria
B) Different path per traffic class
C) Both techniques
D) Routing unrelated to ACL

**Answer: C**

---

### Q65: ACL for anomaly detection (traffic patterns):
A) Baseline established via ACL statistics
B) Deviations detected
C) Both monitoring aspects
D) ACL just filters

**Answer: C**

---

### Q66: Implement reflexive ACL (dynamic allow):
A) Response packets auto-permitted
B) Original request matching creates dynamic rule
C) Both statefull behavior
D) No dynamic ACLs

**Answer: C**

---

### Q67: Design ACL with regular expressions:
A) For named list in modern IOS/ASA
B) Port ranges with regex
C) Limited regex support
D) No regex in ACL

**Answer: C**

---

### Q68: ACL performance impact:
A) More rules = slower processing
B) Hardware ACL optimized
C) Both factors
D) No performance impact

**Answer: C**

---

### Q69: Implement ACL for multi-cloud:
A) Different ACLs per cloud provider
B) Traffic steering by destination
C) Both approaches
D) Single ACL for all

**Answer: C**

---

### Q70: Design ACL for network baseline (acceptable use policy):
A) Define allowed ports/IPs
B) Monitor compliance
C) Both governance elements
D) No policy needed

**Answer: C**

---

## COMMAND REFERENCE

```
! Create standard ACL
access-list 1 permit 192.168.1.0 0.0.0.255
access-list 1 deny any

! Create extended ACL
access-list 101 permit tcp 192.168.1.0 0.0.0.255 any eq 80
access-list 101 permit tcp any any eq 443

! Named standard ACL (modern)
ip access-list standard CompanyNet
 permit 192.168.1.0 0.0.0.255
 deny any
exit

! Named extended ACL (modern)
ip access-list extended FilterHTTP
 permit tcp 10.0.0.0 0.0.0.255 any eq 80
 permit tcp 10.0.0.0 0.0.0.255 any eq 443
 deny ip any any log
exit

! Apply ACL to interface (inbound)
interface FastEthernet0/0
 ip access-group 101 in
exit

! Apply ACL to interface (outbound)
interface FastEthernet0/0
 ip access-group 101 out
exit

! View ACL
show access-lists
show access-lists 101
show ip access-lists

! View ACL on interface
show ip interface FastEthernet0/0 | include access list

! Remove ACL from interface
interface FastEthernet0/0
 no ip access-group 101 in
exit

! Delete entire ACL
no access-list 101

! Modify named ACL (add/delete lines)
ip access-list extended FilterHTTP
 15 permit tcp 172.16.0.0 0.0.0.255 any eq 443
 no 20  ! Delete line 20
exit

! ACL with logging
access-list 101 permit tcp any any eq 80 log
access-list 101 deny ip any any log-input

! ACL for specific host
access-list 101 permit tcp host 192.168.1.1 any eq 22

! ACL with port range
access-list 101 permit tcp any any range 80 443

! ACL with established connections (TCP)
access-list 101 permit tcp any any established

! ACL with ICMP
access-list 102 permit icmp any any

! Delete specific line in named ACL
ip access-list extended FilterHTTP
 no 15
exit

! Reflexive ACL (stateful)
ip access-list extended OutboundTraffic
 permit tcp any any eq 80 reflect HTTP
exit

ip access-list extended InboundTraffic
 permit tcp any any eq 80 evaluated HTTP
exit

! IPv6 ACL
ipv6 access-list AllowHTTP
 permit tcp any any eq 80
exit

! View ACL statistics
show access-lists 101
```

---

## KEY CONCEPTS

1. **Standard ACL**: Filters by source IP only (1-99)
2. **Extended ACL**: Filters by source, destination, protocol, port (100-199)
3. **Named ACL**: Uses names instead of numbers (modern approach)
4. **Wildcard Mask**: Inverted subnet mask (1=ignore, 0=match)
5. **Implicit Deny**: All traffic not matching any rule is denied by default
6. **First Match Wins**: Rules evaluated top-to-bottom
7. **Access Group**: Applied to interface (in/out direction)
8. **Log Keyword**: Records matching packets to syslog
9. **Established Keyword**: Permits TCP responses/return traffic
10. **Any/Host**: Shorthand for addresses
11. **Port Operators**: eq (equal), gt (greater), lt (less), range (inclusive)
12. **Inbound ACL**: Checked before routing (more CPU efficient)
13. **Outbound ACL**: Checked after routing (more rules apply)
14. **Stateful/Reflexive ACL**: Tracks connections and auto-permits response traffic
15. **VLAN ACL**: Filters within/between VLANs on switches (VACL)

