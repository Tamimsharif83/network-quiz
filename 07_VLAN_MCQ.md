# VLAN (Virtual Local Area Network) MCQ Quiz

---

## EASY LEVEL

### Q1: What is a VLAN?
A) Virtual network isolated at Layer 2
B) A way to segment network broadcast domains
C) Logical grouping of ports on switch
D) All of above

**Answer: D**

---

### Q2: Default VLAN number on Cisco switch:
A) VLAN 1
B) VLAN 0
C) VLAN 100
D) None

**Answer: A**

---

### Q3: Create VLAN on switch:
A) `vlan 10`
B) `create vlan 10`
C) `configure vlan 10`
D) `vlan number 10`

**Answer: A**

---

### Q4: Assign port to VLAN:
A) `switchport access vlan 10` (at interface)
B) `vlan 10 ports Fa0/1`
C) `interface vlan 10`
D) Not possible in one command

**Answer: A**

---

### Q5: View configured VLANs:
A) `show vlan`
B) `show vlan brief`
C) Both show VLAN info
D) `show vlans`

**Answer: C**

---

### Q6: VLAN ID range (standard):
A) 1-1024
B) 1-4094
C) 1-4096
D) 0-255

**Answer: B**

---

### Q7: Access mode port vs Trunk:
A) Access = one VLAN, Trunk = multiple VLANs
B) Trunk uses 802.1Q tagging
C) Both correct distinctions
D) Same functionality

**Answer: C**

---

### Q8: Configure trunk port:
A) `switchport mode trunk`
B) `switchport trunk encapsulation dot1q`
C) Both commands for full config
D) Single command sufficient

**Answer: C**

---

### Q9: Allowed VLANs on trunk:
A) `switchport trunk allowed vlan add 20,30`
B) All VLANs by default
C) Specific VLANs configurable
D) All approaches

**Answer: D**

---

### Q10: Native VLAN on trunk (untagged):
A) Always VLAN 1 by default
B) Configurable
C) Both true
D) No native VLAN concept

**Answer: C**

---

### Q11: 802.1Q vs ISL tagging:
A) 802.1Q = Cisco proprietary
B) ISL = standard
C) 802.1Q = standard, ISL = Cisco legacy
D) Both same

**Answer: C**

---

### Q12: Create VLAN interface (SVI):
A) `interface vlan 10`
B) Assign IP address
C) Both steps for management
D) `vlan interface 10`

**Answer: C**

---

### Q13: View VLAN membership of port:
A) `show interface Fa0/1 switchport`
B) Shows access/trunk mode
C) Both show configuration
D) `show port vlan`

**Answer: C**

---

### Q14: VLAN tagging purpose:
A) Identifies VLAN when crossing trunk
B) Switch knows VLAN without tag in same switch
C) Both scenarios
D) No tagging necessary

**Answer: C**

---

### Q15: Inter-VLAN routing requirement:
A) Router between VLANs
B) VLAN routing interfaces needed
C) Both prerequisites
D) Switches route automatically

**Answer: C**

---

### Q16: Delete VLAN:
A) `no vlan 10`
B) `delete vlan 10`
C) `vlan 10 delete`
D) Cannot delete - permanent

**Answer: A**

---

### Q17: Maximum VLANs practical on switch:
A) Limited by hardware/memory
B) 4094 theoretical maximum
C) Depends on switch model
D) All factors

**Answer: D**

---

### Q18: Port security for VLAN:
A) Can configure per VLAN
B) Per-port maximum MAC count
C) Both possible configurations
D) Global setting only

**Answer: C**

---

### Q19: VLAN pruning purpose:
A) Reduces unnecessary traffic on trunk
B) Prevents VLAN from reaching trunk
C) Both benefits
D) Not a common feature

**Answer: C**

---

### Q20: Default trunk native VLAN change:
A) `switchport trunk native vlan 1`
B) Security risk if mismatch
C) Both true
D) No need to change

**Answer: C**

---

## MEDIUM LEVEL

### Q21: Configure VLAN with specific name:
A) `vlan 10` then `name Sales`
B) Both steps needed
C) `vlan 10 name Sales` (single command)
D) Names not supported

**Answer: A**

---

### Q22: Multiple access ports to same VLAN:
A) Assign each individually
B) Range command: `interface range Fa0/1-10`
C) Both possible
D) Must use special config

**Answer: C**

---

### Q23: VLAN trunking protocol (VTP):
A) Synchronizes VLAN info across switches
B) Server/Client/Transparent modes
C) Both features
D) Deprecated

**Answer: C**

---

### Q24: Configure inter-VLAN routing (router-on-stick):
A) Router with multiple subinterfaces
B) Each subinterface = one VLAN
C) Both aspects
D) Not recommended

**Answer: C**

---

### Q25: Subinterface for VLAN 20 on Fa0/0.20:
A) `encapsulation dot1q 20`
B) `ip address 192.168.20.1 255.255.255.0`
C) Both steps
D) `ip vlan 20`

**Answer: C**

---

### Q26: View all subinterfaces and VLANs:
A) `show interfaces subinterfaces`
B) `show ip interface brief`
C) Both show relevant info
D) `show vlan subinterface`

**Answer: C**

---

### Q27: VLAN hopping attack prevention:
A) Disable auto trunk negotiation (DTP)
B) Configure native VLAN mismatch wrong
C) Both prevention methods
D) Not a concern

**Answer: C**

---

### Q28: Configure spanning tree per VLAN (PVST+):
A) Standard in modern switches
B) Per-VLAN STP calculation
C) Both true
D) RSTP always used

**Answer: C**

---

### Q29: VLAN trunking on LAG (EtherChannel):
A) Trunk VLANs across grouped ports
B) Increases bandwidth per VLAN
C) Both benefits
D) Not supported

**Answer: C**

---

### Q30: Voice VLAN and Data VLAN:
A) IP phone on access port with voice VLAN config
B) Computer on same port in data VLAN
C) Both possible
D) Separate ports required

**Answer: C**

---

### Q31: Configure voice VLAN:
A) `switchport voice vlan 100`
B) At interface level
C) Both true
D) `voice-vlan 100`

**Answer: C**

---

### Q32: VLAN in multi-switch environment:
A) Trunks propagate VLAN membership
B) Port configuration per switch needed
C) Both required efforts
D) All automatic

**Answer: C**

---

### Q33: Allowed VLAN list on trunk (all except):
A) `switchport trunk allowed vlan all`
B) `except 1,1002-1005`
C) Both syntax available
D) Must explicitly list

**Answer: C**

---

### Q34: MAC address table per VLAN:
A) Yes - separate per VLAN
B) Global table
C) Depends on implementation
D) No MAC table

**Answer: A**

---

### Q35: Dynamic trunk negotiation (DTP):
A) Auto-negotiates trunk
B) Security risk (can be exploited)
C) Both true
D) Always enabled

**Answer: C**

---

### Q36: Disable DTP (static trunk):
A) `switchport mode trunk`
B) `switchport nonegotiate`
C) Both disable negotiation
D) `no negotiation`

**Answer: C**

---

### Q37: VLAN management interface (VLAN 1):
A) Special status
B) Can't delete typically
C) Both characteristics
D) Like any other VLAN

**Answer: C**

---

### Q38: Link-local multicast address behavior on VLAN:
A) Contained within VLAN
B) Router required to forward
C) Both true
D) Automatically propagates

**Answer: C**

---

### Q39: Private VLAN (PVLAN):
A) Subtype communities within secondary VLAN
B) Isolated/promiscuous ports
C) Both features
D) Not a real feature

**Answer: C**

---

### Q40: Broadcast suppression per VLAN:
A) Can limit broadcast traffic
B) Useful for congestion control
C) Both true
D) Automatic - no config

**Answer: C**

---

## HARD LEVEL

### Q41: Design VLAN architecture for enterprise (100+ VLANs):
A) Organizational based
B) Department + site hierarchy
C) Layer 2/3 boundary planning
D) All considerations

**Answer: D**

---

### Q42: VLAN security with 802.1X:
A) Port-based authentication
B) VLAN assignment post-auth
C) Both mechanisms
D) Not compatible

**Answer: C**

---

### Q43: Implement private VLAN with guest isolation:
A) Guest in secondary isolated community
B) Can reach gateway/resources selective
C) Both design aspects
D) Not practical

**Answer: C**

---

### Q44: VLAN with STP topology:
A) Root bridge per VLAN (PVST+)
B) Eliminates loops per VLAN
C) Both mechanisms
D) STP ignores VLANs

**Answer: C**

---

### Q45: Design VLAN trunking strategy:
A) Mesh trunk fully connected
B) Star topology with core hub
C) Depends on scalability needs
D) Either approach valid

**Answer: D**

---

### Q46: VLAN configuration synchronization via VTP:
A) Server authoritative
B) Client learns from server
C) Transparent mode also exists
D) All modes described

**Answer: D**

---

### Q47: Implement VLAN for different security zones:
A) DMZ, Internal, Guest VLANs
B) Policies enforced via access-lists
C) Both design elements
D) VLANs sufficient alone

**Answer: C**

---

### Q48: VLAN in datacenter (convergence):
A) VLANs carry storage traffic
B) Different VLANs per traffic type
C) Both practices
D) VLANs not used in DC

**Answer: C**

---

### Q49: Design VLAN for high availability:
A) Redundant spanning tree
B) Multiple trunks between switches
C) Rapid STP convergence
D) All HA elements

**Answer: D**

---

### Q50: VLAN in wireless networks:
A) SSID per VLAN group
B) Client VLAN assignment dynamic
C) Both scenarios
D) VLANs not for wireless

**Answer: C**

---

### Q51: Implement QoS per VLAN:
A) Service classes per VLAN
B) Traffic shaping capabilities
C) Both features
D) No per-VLAN QoS

**Answer: C**

---

### Q52: VLAN design for guest network:
A) Isolated VLAN
B) Limited internet access only
C) Both security measures
D) Full network access standard

**Answer: C**

---

### Q53: Configure VLAN stacking (QinQ):
A) Double tagging for service provider
B) Inner VLAN preserved through provider
C) Both aspects
D) Not supported

**Answer: C**

---

### Q54: Design VLAN for IoT devices:
A) Separate VLAN for devices
B) Segmented access control
C) Both security practices
D) No special handling

**Answer: C**

---

### Q55: VLAN 802.1ad (provider bridges):
A) Service provider tagging
B) Two-level hierarchy
C) Both concepts
D) Cisco proprietary

**Answer: C**

---

### Q56: Implement VLAN with MAC-based assignment:
A) Dynamic MAC-to-VLAN mapping
B) Switch learns and applies
C) Both dynamic features
D) Manual-only assignment

**Answer: C**

---

### Q57: Design VLAN for network convergence (voice/video/data):
A) Separate VLANs per traffic type
B) Priority queuing configured
C) Both optimization strategies
D) Single VLAN sufficient

**Answer: C**

---

### Q58: VLAN security in multi-tenant (cloud):
A) Per-tenant VLAN isolation
B) No leakage between customers
C) Both requirements
D) VLANs insufficient for cloud

**Answer: C**

---

### Q59: Implement LACP trunk with VLAN:
A) Load-balance across link aggregation
B) Same VLANs on all links
C) Both benefits
D) Incompatible with VLANs

**Answer: C**

---

### Q60: Design VLAN for disaster recovery:
A) Production and backup VLANs separate
B) Failover capability built in
C) Both elements
D) No special VLAN design

**Answer: C**

---

### Q61: Configure VLAN in multi-layer architecture:
A) Access layer ports in VLANs
B) Distribution/core aggregation with trunking
C) Both layers involved
D) VLANs only at access

**Answer: C**

---

### Q62: VLAN QoS marking (802.1p/CoS):
A) Priority levels per VLAN
B) Traffic classification enabled
C) Both features
D) No QoS in VLANs

**Answer: C**

---

### Q63: Design VLAN for network monitoring:
A) SPAN (Switched Port Analyzer) per VLAN
B) Mirror traffic to monitoring port
C) Both monitoring capabilities
D) Not possible per VLAN

**Answer: C**

---

### Q64: Implement selective VLAN pruning:
A) Removes unnecessary VLAN from trunk
B) Reduces unnecessary traffic
C) Both benefits
D) All VLANs always on trunk

**Answer: C**

---

### Q65: VLAN consistency across campus network:
A) Standardized VLAN numbering
B) Documentation and automation
C) Both practices
D) No special consideration

**Answer: C**

---

### Q66: Configure VLAN with static and dynamic assignment:
A) Some ports static to VLAN
B) Others dynamic via 802.1X/RADIUS
C) Both possible
D) Only one method per switch

**Answer: C**

---

### Q67: Design VLAN for real-time applications:
A) Low-latency VLAN dedicated
B) Priority queuing configured
C) Both optimization elements
D) Standard VLAN sufficient

**Answer: C**

---

### Q68: VLAN in software-defined network (SDN):
A) Dynamic VLAN assignment
B) Central controller managed
C) Both SDN features
D) VLANs not used in SDN

**Answer: C**

---

### Q69: Implement VLAN firewall policies:
A) ACLs per VLAN
B) Policies enforced between VLANs
C) Both security layers
D) VLANs = no firewall needed

**Answer: C**

---

### Q70: Design VLAN for regulatory compliance:
A) PCI-DSS VLANs separation
B) Audit trails and logging
C) Both compliance measures
D) No special VLAN design needed

**Answer: C**

---

## COMMAND REFERENCE

```
! Create VLAN
vlan 10
 name Sales
exit

! View VLANs
show vlan
show vlan brief
show vlan id 10

! Assign port to access VLAN
interface FastEthernet0/1
  switchport mode access
  switchport access vlan 10
exit

! Configure trunk port
interface GigabitEthernet0/1
  switchport mode trunk
  switchport trunk encapsulation dot1q
  switchport trunk allowed vlan 1,10,20,30
  switchport trunk native vlan 1
exit

! Configure VLAN interface (SVI)
interface vlan 10
  ip address 192.168.10.1 255.255.255.0
  no shutdown
exit

! Configure subinterface for inter-VLAN routing
interface FastEthernet0/0.10
  encapsulation dot1q 10
  ip address 192.168.10.254 255.255.255.0
exit

interface FastEthernet0/0.20
  encapsulation dot1q 20
  ip address 192.168.20.254 255.255.255.0
exit

! Voice VLAN
interface FastEthernet0/2
  switchport mode access
  switchport access vlan 100  ! Data
  switchport voice vlan 110   ! Voice
exit

! Delete VLAN
no vlan 10

! Port security per VLAN
interface FastEthernet0/1
  switchport port-security
  switchport port-security maximum 5
  switchport port-security violation protect
exit

! Private VLAN
vlan 100
 private-vlan primary
exit
vlan 101
 private-vlan isolated
exit

interface FastEthernet0/1
 switchport mode private-vlan host
 switchport private-vlan host-association 100 101
exit

! Multiple ports to VLAN
interface range FastEthernet0/1-10
  switchport access vlan 10
exit

! View port switchport config
show interfaces FastEthernet0/1 switchport
```

---

## KEY CONCEPTS

1. **VLAN**: Logical segmentation of network (Layer 2 isolation)
2. **Broadcast Domain**: Devices in VLAN receive each other's broadcasts
3. **802.1Q Tagging**: Standard method of identifying VLAN on trunk
4. **Native VLAN**: Untagged traffic on trunk (default VLAN 1)
5. **Access Mode**: Port belongs to single VLAN
6. **Trunk Mode**: Port carries multiple VLANs (tagged)
7. **SVI (VLAN Interface)**: Virtual interface for a VLAN (IP assignment)
8. **Inter-VLAN Routing**: Router routes between VLANs
9. **VLAN ID**: 1-4094 (1-1005 standard, 1006-4094 extended)
10. **VTP (VLAN Trunking Protocol)**: Synchronizes VLAN info (Server/Client/Transparent)
11. **Spanning Tree per VLAN (PVST+)**: Separate STP instance per VLAN
12. **VLAN Pruning**: Prevents unnecessary broadcasts on trunk
13. **Port Security**: Limit MAC addresses per port/VLAN
14. **Private VLAN**: Subset isolation for specific groups
15. **DTP (Dynamic Trunking Protocol)**: Auto-negotiates trunk (security risk)

