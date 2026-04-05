# OSPF (Open Shortest Path First) MCQ Quiz

---

## EASY LEVEL

### Q1: What does OSPF stand for?
A) Open Shortest Path First
B) Open Source Path Finding
C) Open Speed Path First
D) Open Segment Protocol First

**Answer: A**

---

### Q2: OSPF administrative distance:
A) 90
B) 100
C) 110
D) 120

**Answer: C**

---

### Q3: OSPF uses which routing algorithm?
A) Bellman-Ford
B) Dijkstra's SPF (Shortest Path First)
C) RTA
D) BGP-like

**Answer: B**

---

### Q4: Enable OSPF process:
A) `router ospf 1`
B) `ospf 1`
C) `enable ospf 1`
D) `configure ospf 1`

**Answer: A**

---

### Q5: Configure network in OSPF area:
A) `network 192.168.1.0 area 0`
B) `network 192.168.1.0 255.255.255.0 area 0`
C) `network 192.168.1.0 0.0.0.255 area 0`
D) C is correct (wildcard mask)

**Answer: C**

---

### Q6: OSPF backbone area number:
A) Area 0
B) Area 1
C) Area default
D) Area 255

**Answer: A**

---

### Q7: OSPF hello packet interval:
A) 5 seconds
B) 10 seconds
C) 30 seconds
D) 60 seconds

**Answer: B**

---

### Q8: OSPF dead timer (default):
A) Hello timeout
B) 4 × hello interval
C) 30 seconds
D) 40 seconds

**Answer: B**

---

### Q9: View OSPF neighbors:
A) `show ospf neighbors`
B) `show ip ospf neighbors`
C) `show ospf routers`
D) `show protocols neighbors`

**Answer: B**

---

### Q10: OSPF neighbor states in order (first to last):
A) Down → Full
B) Down → Init → ExStart → Exchange → Loading → Full
C) Down → Full directly
D) Order doesn't matter

**Answer: B**

---

### Q11: OSPF router with lowest Router ID becomes:
A) Primary
B) Designated Router (DR) in broadcast segment
C) Backup DR
D) No special role

**Answer: B**

---

### Q12: OSPF Router ID (if not set manually):
A) Lowest interface IP
B) Highest interface IP
C) Highest loopback IP
D) Any interface randomly

**Answer: C**

---

### Q13: Manually configure OSPF Router ID:
A) `router-id 1.1.1.1`
B) At OSPF config level
C) Both
D) `ospf router-id 1.1.1.1`

**Answer: C**

---

### Q14: OSPF metric/cost based on:
A) Hop count
B) Interface bandwidth
C) Delay
D) 100,000 / bandwidth (Mbps)

**Answer: D**

---

### Q15: Modify interface cost in OSPF:
A) `cost 50` (at interface)
B) `ip ospf cost 50`
C) Both
D) Not possible

**Answer: B**

---

### Q16: View OSPF database:
A) `show ip ospf database`
B) `show ospf lsa`
C) Both
D) `show database ospf`

**Answer: C**

---

### Q17: LSA type 1:
A) Router LSA
B) Network LSA
C) Summary LSA
D) External LSA

**Answer: A**

---

### Q18: Passive interface in OSPF:
A) Doesn't send hello
B) Neighbor won't form
C) Network is still advertised
D) All above

**Answer: D**

---

### Q19: Configure passive interface:
A) `passive-interface Serial0/0`
B) At OSPF level or interface level
C) Both approaches
D) `no ospf hello` (old syntax)

**Answer: C**

---

### Q20: View OSPF configuration / parameters:
A) `show ip ospf`
B) `show ip protocols`
C) Both show relevant info
D) `show ospf parameters`

**Answer: C**

---

## MEDIUM LEVEL

### Q21: Configure OSPF area with wildcard/mask:

A) `network 10.0.0.0 0.255.255.255 area 0`
B) Matches interfaces in range
C) Both true
D) Mask inverted (1=match, 0=don't care)

**Answer: A**

---

### Q22: OSPF stub area - cannot contain:
A) External routes (Type 5 LSA)
B) ASBR (Autonomous System Boundary Router)
C) Both - no external routes or ASBR
D) Can contain both

**Answer: C**

---

### Q23: Configure stub area (traditional):
A) `area 1 stub` (at area config)
B) All routers in area must agree
C) Both requirements
D) No special command needed

**Answer: C**

---

### Q24: OSPF totally stubby area:
A) No external routes
B) No summary routes from other areas
C) Both restrictions
D) Not a standard term

**Answer: C**

---

### Q25: Configure ABR (Area Border Router):
A) Manually designate
B) Automatically detected (has routers in multiple areas)
C) Requires special config
D) `area-border-router` command

**Answer: B**

---

### Q26: OSPF virtual link - when used:
A) Connecting discontiguous areas
B) Area without backbone connectivity
C) Temporary link via transit area
D) All correct scenarios

**Answer: D**

---

### Q27: Configure OSPF virtual link:
A) `area 1 virtual-link 2.2.2.2`
B) At OSPF config
C) Both must exist in configuration
D) Requires special hardware

**Answer: C**

---

### Q28: OSPF authentication (simple/MD5):
A) `authentication [md5] simple` (area level)
B) `authentication-key / message-digest-key` (interface level)
C) Both configurations
D) Only key-chain method

**Answer: C**

---

### Q29: OSPF redistribution into area:
A) `redistribute static` (at OSPF level)
B) Creates Type 5 LSA (forwarding address)
C) Both
D) Only via ASBR

**Answer: C**

---

### Q30: Configure default route origination in OSPF:
A) `default-information originate`
B) `always` parameter forces advertisement even if not in table
C) Both options available
D) Only works with stub areas

**Answer: C**

---

### Q31: OSPF route summarization at ABR:
A) `area 1 range 192.168.0.0 255.255.0.0`
B) Suppresses component LSAs
C) Both benefits
D) For inter-area routes

**Answer: D**

---

### Q32: View OSPF SPF calculation timer:
A) `show ip ospf` shows SPF runs
B) `debug ospf spf` traces calculations
C) Both reveal information
D) SPF is automatic, not shown

**Answer: C**

---

### Q33: OSPF point-to-point network type:
A) No DR/BDR elected
B) Sends hello as multicast
C) MTU mismatch dangerous
D) All apply to P2P

**Answer: D**

---

### Q34: Change OSPF network type:
A) `ip ospf network broadcast/point-to-point/point-to-multipoint`
B) At interface level
C) Both
D) Not configurable

**Answer: C**

---

### Q35: OSPF broadcast network - maximum useful routers:
A) Any number (no limit)
B) 5-10 (DR/BDR overhead)
C) 255
D) 256

**Answer: B**

---

### Q36: Configure OSPF timers:
A) `timers hello 20` (at interface)
B) `timers dead 80`
C) Both configurable per interface
D) Global config only

**Answer: C**

---

### Q37: OSPF cost calculator for Ethernet:
A) Formula: 100Mbps / interface bandwidth
B) 10 Mbps = cost 10
C) 100 Mbps = cost 1
D) All calculations

**Answer: D**

---

### Q38: Modify OSPF reference bandwidth:
A) `auto-cost reference-bandwidth 1000`
B) Changes calculation for all interfaces
C) Used when link > 100Mbps
D) All correct

**Answer: D**

---

### Q39: OSPF process restart impact:
A) Neighbors removed, full SPF recalculation
B) Temporary disruption (depends on timers)
C) Both consequences
D) No disruption with NSF

**Answer: D**

---

### Q40: Clear OSPF neighbor / database:
A) `clear ip ospf process`
B) `clear ip ospf neighbor`
C) Both available
D) `restart ospf`

**Answer: C**

---

## HARD LEVEL

### Q41: Design OSPF multi-area with backbone:
A) Area 0 as backbone
B) ABRs connect areas to backbone
C) No area-to-area communication bypassing backbone
D) All architectural rules

**Answer: D**

---

### Q42: Implement OSPF NSSA (Not-So-Stubby Area):
A) Accepts external routes (Type 7 LSA)
B) ASBR needs special configuration
C) Type 7 converted to Type 5 at ABR
D) All correct

**Answer: D**

---

### Q43: Configure NSSA area to accept external:
A) `area 1 nssa`
B) Routers advertise external via Type 7
C) Both conditions
D) ABR automatic conversion

**Answer: D**

---

### Q44: OSPF converge time characteristics:
A) Based on SPF calculation interval
B) Faster than RIPv2 (v1 much slower)
C) Hello/dead timers factor in
D) All factors affect speed

**Answer: D**

---

### Q45: Implement OSPF fast failover (sub-second):
A) Adjust hello/dead timers lower
B) Enable BFD (Bidirectional Forwarding Detection)
C) Multiple equal-cost paths present
D) All mechanisms

**Answer: D**

---

### Q46: OSPF with unequal-cost load balancing:
A) Not supported (only equal-cost)
B) Alternative path in table if better
C) Both characterize limitation
D) Limited to equal-cost multipath

**Answer: D**

---

### Q47: Design hub-and-spoke OSPF:
A) Hub in area 0, spokes in areas 1, 2...
B) All spokes have default route from ABR
C) Reduces routing updates at spokes
D) All design elements

**Answer: D**

---

### Q48: Implement prefix filtering in OSPF:
A) `distribute-list IN/OUT`
B) Route-map based filtering
C) Both mechanisms available
D) Limited to LSA suppression

**Answer: C**

---

### Q49: OSPF graceful restart (NSF):
A) Preserves neighbor adjacencies
B) Kernel continues forwarding
C) Both processes coordinated
D) All aspects

**Answer: D**

---

### Q50: OSPF with traffic engineering (MPLS TE):
A) Links advertise bandwidth constraints
B) Path calculation includes TE metrics
C) TE tunnels preferred for traffic
D) All features

**Answer: D**

---

### Q51: Configure OSPF demand circuit:
A) BGP-like behavior (no periodic updates)
B) Useful for expensive links (dial-on-demand)
C) Both true
D) OSPF always sends updates

**Answer: C**

---

### Q52: OSPF area summarization (ABR):
A) Type 3 LSA (summary)
B) Reduces routing table at routers
C) Both benefits
D) Only in Area 0

**Answer: C**

---

### Q53: Design OSPF in MPLS environment:
A) OSPF independent of MPLS
B) Routing and forwarding decoupled
C) Both architecture points
D) MPLS requires BGP only

**Answer: C**

---

### Q54: Implement OSPF for service provider:
A) Single large area (flat topology)
B) Multiple smaller areas with hierarchy
C) B for scalability preference
D) Depends on network size

**Answer: C**

---

### Q55: OSPF LSA aging (MaxAge):
A) 3600 seconds
B) Removed from database after expiry
C) Refreshed by originator
D) All correct

**Answer: D**

---

### Q56: Configure OSPF authentication with key-chain:
A) `area 0 authentication [md5]`
B) Interface: `ip ospf authentication key-chain`
C) Both levels of config
D) Key-chain not supported in OSPF

**Answer: C**

---

### Q57: Design OSPF with redundancy:
A) Multiple paths to destination
B) Equal-cost or unequal via higher AD alternate
C) BFD for fast detection
D) All redundancy techniques

**Answer: D**

---

### Q58: OSPF between vendors (interop):
A) Standardized (RFC 2328)
B) Most vendor-compatible routing protocol
C) Both true
D) Limited interoperability

**Answer: B**

---

### Q59: Implement OSPF in VRF:
A) Separate OSPF process per VRF
B) No route leakage between VRFs
C) Both apply
D) Single OSPF for all VRFs

**Answer: C**

---

### Q60: OSPF cost metric optimization:
A) Default metric on Gigabit = 1
B) On 10 Mbps = 10
C) Artificially adjust for traffic engineering
D) All methods

**Answer: D**

---

### Q61: Implement OSPF prefix filtering on export:
A) `distribute-list 1 out Interface`
B) With access-list filtering
C) Prevents LSA generation
D) All aspects

**Answer: D**

---

### Q62: Design OSPF for disaster recovery (active-backup):
A) Primary converges via OSPF
B) Backup via manual intervention or alternate protocol
C) Fast convergence preferred
D) All design points

**Answer: D**

---

### Q63: OSPF in highly redundant mesh:
A) Multiple paths automatically load-balanced
B) Equal-cost multipath without explicit config
C) Converges to shortest paths
D) All advantages

**Answer: D**

---

### Q64: Implement OSPF inter-area multicast:
A) OSPF carries multicast routing info
B) Builds shared trees across areas
C) Type 3 LSA carries multicast
D) DVMRP/PIM for multicast, separate from OSPF unicast

**Answer: D**

---

### Q65: OSPF graceful shutdown (route withdrawal):
A) Send LSA with infinite cost (metric=largest)
B) Immediate neighbor removal
C) Withdrawal via MaxAge LSA
D) All mechanisms

**Answer: D**

---

### Q66: Configure OSPF for low-bandwidth links (e.g., 64kbps):
A) Increase hello/dead timers
B) Decrease cost artificially
C) Both optimizations
D) Default timers fine

**Answer: C**

---

### Q67: OSPF database overflow protection:
A) LSA limiting per area
B) Prevent memory exhaustion attacks
C) Both security protections
D) Unlimited LSAs accepted

**Answer: C**

---

### Q68: Design OSPF aggregation strategy:
A) Summarize at area boundaries (ABR)
B) External routes at ASBR
C) Both aggregation points
D) No aggregation possible

**Answer: C**

---

### Q69: OSPF convergence comparison (to EIGRP/RIPv2):
A) Generally faster than RIPv2
B) Comparable to EIGRP (both sub-second capable)
C) Both accurate
D) Slower than both

**Answer: C**

---

### Q70: Implement OSPF for global network:
A) Single AS with multiple areas
B) Super-areas not standard in OSPF
C) Both characterize OSPF limits
D) Requires BGP for true global scale

**Answer: D**

---

## COMMAND REFERENCE

```
! Enable OSPF process
router ospf 1

! Configure network (wildcard mask)
network 10.0.0.0 0.255.255.255 area 0
network 192.168.0.0 0.0.255.255 area 1

! View OSPF neighbors
show ip ospf neighbors
show ip ospf neighbors detail

! View OSPF topology database
show ip ospf database
show ip ospf database router
show ip ospf database summary

! View OSPF routes
show ip route ospf

! Set Router ID
router ospf 1
  router-id 1.1.1.1
exit

! Interface cost
interface GigabitEthernet0/0
  ip ospf cost 50
exit

! Configure hello and dead timers
interface Serial0/0
  ip ospf hello-interval 10
  ip ospf dead-interval 40
exit

! Passive interface
passive-interface Serial0/0
passive-interface default

! Configure stub area
router ospf 1
  area 1 stub
exit

! Configure NSSA area
router ospf 1
  area 2 nssa
exit

! Area summarization (ABR)
router ospf 1
  area 1 range 192.168.0.0 255.255.0.0
exit

! Default route origination
router ospf 1
  default-information originate
exit

! Configure network type
interface Serial0/0
  ip ospf network point-to-point
exit

! OSPF authentication (simple)
interface Ethernet0/0
  ip ospf authentication-key MyPassword
exit

router ospf 1
  area 0 authentication
exit

! OSPF MD5 authentication
interface Ethernet0/0
  ip ospf message-digest-key 1 md5 MySecureKey
exit

router ospf 1
  area 0 authentication message-digest
exit

! Virtual link
router ospf 1
  area 1 virtual-link 2.2.2.2
exit

! Redistribute external routes
router ospf 1
  redistribute static subnets
  redistribute bgp 65000 subnets
exit

! Configure reference bandwidth
router ospf 1
  auto-cost reference-bandwidth 10000
exit

! Distribute list (route filtering)
distribute-list 1 in Serial0/0
distribute-list 2 out FastEthernet0/0

! Clear OSPF
clear ip ospf process
clear ip ospf neighbor

! View OSPF configuration
show ip ospf
show ip protocols
show running-config | section ospf
```

---

## KEY CONCEPTS

1. **SPF (Shortest Path First)**: Dijkstra algorithm core of OSPF
2. **Area Concept**: Hierarchical network organization
3. **Backbone Area (Area 0)**: Central area connecting all other areas
4. **Designated Router (DR)**: Elected router in broadcast segment for adjacencies
5. **LSA (Link State Advertisement)**: Database entry (Type 1-5)
6. **ABR (Area Border Router)**: Connects multiple areas
7. **ASBR (Autonomous System Boundary)**: Redistributes external routes
8. **Stub Area**: No external routes (Type 5 LSA)
9. **NSSA (Not-So-Stubby)**: Accepts external routes as Type 7 LSA
10. **Virtual Link**: Connects discontiguous areas through transit area
11. **Network Types**: Broadcast, Point-to-Point, Point-to-Multipoint, NBMA
12. **Cost/Metric**: Bandwidth-based (100Mbps reference / interface bandwidth)
13. **Authentication**: Simple or MD5 per area
14. **Demand Circuit**: Designed for expensive links (no periodic updates)
15. **Convergence**: SPF calculation time + hello/dead intervals (typically <1 second with BFD)

