# EIGRP (Enhanced Interior Gateway Routing Protocol) MCQ Quiz

---

## EASY LEVEL

### Q1: What does EIGRP stand for?
A) Enhanced Interior Gateway Routing Protocol
B) Exterior Interior Gateway Route Protocol
C) Equipment Interior Gateway Routing Protocol
D) Enhanced Integrated Gateway Route Protocol

**Answer: A**

---

### Q2: EIGRP administrative distance (default) for internal routes:
A) 90
B) 100
C) 110
D) 120

**Answer: A**

---

### Q3: EIGRP uses which routing algorithm?
A) Dijkstra's
B) Bellman-Ford
C) Dual (Diffusing Update Algorithm)
D) RTA

**Answer: C**

---

### Q4: Enable EIGRP router process:
A) `router eigrp 1`
B) `enable eigrp 1`
C) `eigrp 1`
D) `configure eigrp 1`

**Answer: A**

---

### Q5: Configure network in EIGRP:
A) `network 192.168.1.0`
B) `network 192.168.1.0 255.255.255.0`
C) `network 192.168.1.0 0.0.0.255` (wildcard)
D) All formats valid

**Answer: C**

---

### Q6: EIGRP neighbor discovery via:
A) Hello packets
B) Multicast 224.0.0.10
C) Both A and B
D) Unicast only

**Answer: C**

---

### Q7: EIGRP hello interval (default):
A) 5 seconds
B) 10 seconds
C) 30 seconds
D) 60 seconds

**Answer: B**

---

### Q8: EIGRP hold time (default):
A) 15 seconds
B) 30 seconds
C) 45 seconds
D) 60 seconds

**Answer: B**

---

### Q9: View EIGRP neighbors:
A) `show eigrp neighbors`
B) `show ip eigrp neighbors`
C) `show eigrp routers`
D) `show protocols neighbors`

**Answer: B**

---

### Q10: EIGRP metric components - what are they?
A) Bandwidth, Delay
B) Hop count
C) Reliability, Load, MTU
D) All of above

**Answer: D**

---

### Q11: Default EIGRP metric weights K1, K3, K4, K5:
A) All 0
B) K1=1, K3=1, others 0
C) All 1
D) Depends on network

**Answer: B**

---

### Q12: EIGRP successor route - what is it?
A) Best route to destination
B) Backup route
C) Lowest-cost neighbor
D) All neighbors

**Answer: A**

---

### Q13: EIGRP feasible successor - what is it?
A) Next best route
B) Backup neighbor with advertised distance < successor's distance
C) Standby neighbor
D) Any other route

**Answer: B**

---

### Q14: If feasible successor unavailable, EIGRP does what?
A) Immediately routes via neighbor anyway
B) Enters active state, queries neighbors
C) Uses longest-path routing
D) Drops traffic

**Answer: B**

---

### Q15: EIGRP maximum hop count:
A) 15
B) 255
C) Unlimited (up to 224)
D) 256

**Answer: C**

---

### Q16: View EIGRP topology table:
A) `show ip eigrp topology`
B) `show eigrp route`
C) `show route eigrp`
D) `show topology table`

**Answer: A**

---

### Q17: EIGRP passive interface - what does it do?
A) Stops sending updates
B) Stops receiving updates
C) Stops hello packets, stops forming neighbor
D) Interface disabled

**Answer: C**

---

### Q18: View EIGRP configuration:
A) `show ip protocols`
B) `show router eigrp`
C) `show running-config | include eigrp`
D) A or C

**Answer: D**

---

### Q19: Remove EIGRP from router:
A) `no router eigrp 1`
B) `disable eigrp`
C) `shutdown eigrp`
D) `router eigrp 0`

**Answer: A**

---

### Q20: Wildcard mask in EIGRP network command:
A) Matches interfaces that match network+wildcard
B) Different from subnet mask (inverted bits)
C) 0 = must match, 1 = don't care
D) All of above

**Answer: D**

---

## MEDIUM LEVEL

### Q21: Configure EIGRP AS 100 with network 10.0.0.0/8 and 192.168.0.0/16:
A) `router eigrp 100` → `network 10.0.0.0` → `network 192.168.0.0`
B) Both as `/8` and `/16`
C) A is correct for classful-like, but wildcard better
D) `network 10.0.0.0 0.255.255.255` and `network 192.168.0.0 0.0.255.255`

**Answer: D**

---

### Q22: EIGRP on IPv6 networks:
A) Not supported
B) Supported natively as EIGRP for IPv6
C) Requires separate configuration
D) B and C both apply

**Answer: D**

---

### Q23: Configure EIGRP metric K-values:
A) `metric weights 0 1 0 1 0 0`
B) In EIGRP router context
C) Changes how metric calculated
D) All true

**Answer: D**

---

### Q24: EIGRP redistribution command syntax:
A) `redistribute static`
B) `redistribute eigrp 200` (from AS 200)
C) `redistribute connected`
D) All valid

**Answer: D**

---

### Q25: EIGRP route summarization (aggregation):
A) Automatic at network boundary
B) Manual via `summary-address`
C) Creates loopback with summary
D) B for explicit; but A for some topologies

**Answer: B**

---

### Q26: Configure manual EIGRP summary on interface:
A) `ip summary-address eigrp AS NETWORK MASK`
B) At interface level
C) Typical for stub networks
D) All apply

**Answer: D**

---

### Q27: EIGRP load balancing (unequal-cost):
A) `variance 2` multiplier
B) Uses feasible successor if within variance
C) Distributes traffic proportionally
D) All of above

**Answer: D**

---

### Q28: EIGRP query scope - limiting query range:
A) `query-interval`
B) EIGRP queries propagate to all routers (full range)
C) Stub routing limits queries
D) Regional/boundary limiting

**Answer: C**

---

### Q29: Configure EIGRP stub router:
A) `eigrp stub`
B) `eigrp stub connected summary`
C) At router EIGRP config
D) B and C

**Answer: D**

---

### Q30: EIGRP hello timer modification:
A) `hello-interval 5` (on interface)
B) Per-interface setting
C) Changes neighbor timing
D) All true

**Answer: D**

---

### Q31: EIGRP authentication (MD5):
A) `authentication mode md5 key-chain NAME`
B) Per-interface or global
C) Requires key-chain pre-configuration
D) All of above

**Answer: D**

---

### Q32: EIGRP graceful shutdown (GR):
A) `graceful-restart` command
B) Prevents temporary routing disruption
C) Preserves neighbor relationships during restart
D) All correct

**Answer: D**

---

### Q33: Implement EIGRP Leak Map (selective redistribution):
A) `leak-map` feature in newer IOS
B) Prevents route-map blocking on redistribution
C) Routes flow through when conditions met
D) All definitions

**Answer: D**

---

### Q34: EIGRP split horizon:
A) Prevents sending route back to source
B) Disabled by default for some scenarios
C) Applies to feasible successor routes
D) All true

**Answer: D**

---

### Q35: EIGRP default metric for route metric computation:
A) Auto-calculated from interface speed/delay
B) Uses K-values formula
C) Both
D) Preconfigured

**Answer: C**

---

### Q36: View EIGRP peers in detail:
A) `show ip eigrp neighbors detail`
B) Shows Q count, seq num, retrans
C) Both
D) `show eigrp peers`

**Answer: C**

---

### Q37: EIGRP timers (hello, hold):
A) `timers hello 10`
B) `timers hold 30`
C) Can be asymmetric (different on each router)
D) Should match for stability

**Answer: C**

---

### Q38: EIGRP external route - administrative distance:
A) 90 (internal)
B) 170 (external)
C) 110
D) Depends on source

**Answer: B**

---

### Q39: Configure EIGRP offset-list (metric manipulation):
A) `offset-list IN/OUT metric`
B) Apply to interface
C) Increases/decreases route cost
D) All apply

**Answer: D**

---

### Q40: EIGRP feasibility condition:
A) Advertised Distance < Feasible Distance
B) Ensures loop-free alternate paths
C) Enables fast convergence
D) All correct

**Answer: D**

---

## HARD LEVEL

### Q41: Design EIGRP hub-and-spoke with stub routers on spokes:
A) Hubs run full EIGRP, spokes as stub
B) Spoke's `stub connected summary` advertise local networks
C) Reduces query overhead significantly
D) All of above

**Answer: D**

---

### Q42: Implement EIGRP prefix filtering (distribute-list):
A) `distribute-list ROUTE-MAP in/out`
B) Prevents route advertisement/receipt
C) Both
D) Access-list only

**Answer: C**

---

### Q43: EIGRP conditional default route advertisement:
A) `default-information originate [always]`
B) `always` force advertise even if not in table
C) Requires default route exist
D) B applies when option omitted

**Answer: D**

---

### Q44: Configure EIGRP named mode (modern):
A) Named mode vs AS number (legacy)
B) Enhanced configuration flexibility
C) IPv4 and IPv6 in same config
D) All advantages

**Answer: D**

---

### Q45: EIGRP fast convergence mechanism:
A) Feasible successor pre-computed
B) No query flood if FS available
C) Achieves sub-second convergence
D) All true

**Answer: D**

---

### Q46: Implement traffic engineering via EIGRP metrics:
A) Manually set bandwidth/delay on interfaces
B) Influence path selection
C) `bandwidth` command on interface
D) All methods

**Answer: D**

---

### Q47: EIGRP IPv4 and IPv6 coexist on same links?
A) Separate EIGRP processes not possible
B) Named mode allows both
C) Requires dedicated process per protocol
D) Completely separate instances needed

**Answer: B**

---

### Q48: Design EIGRP with area-like hierarchy (EIGRP v6):
A) PITs (Primary Independent Tree)
B) Aggregation at boundaries
C) No true area concept
D) Summarization achieves similar effect

**Answer: D**

---

### Q49: Configure EIGRP prefix suppression (stub):
A) `stub prevent-query`
B) Only export connected/summary
C) Restricts query propagation
D) Advanced stub feature

**Answer: D**

---

### Q50: Implement seamless EIGRP v4→v6 migration:
A) Parallel protocol run
B) Enable IPv6 EIGRP alongside IPv4
C) Redistribute as needed
D) All steps in migration

**Answer: D**

---

### Q51: EIGRP query suppression in converged network:
A) Queries limited to affected nodes
B) Topology redundancy reduces queries
C) Feasible successor available = no query
D) All mechanisms apply

**Answer: D**

---

### Q52: Implement EIGRP graceful restart (preserve state):
A) `graceful-restart [grace-period]`
B) Neighbors don't remove adjacency
C) Routes reinstalled from topology table
D) All correct

**Answer: D**

---

### Q53: EIGRP with BGP route redistribution - AS path implications?
A) EIGRP loses AS path context
B) Requires route-map to preserve
C) Tagging/attributes alternative
D) All considerations

**Answer: D**

---

### Q54: Design multi-region EIGRP with backbone:
A) Hub core, regional spokes
B) Summarization at region boundary
C) Query scoping via stub
D) All architectural elements

**Answer: D**

---

### Q55: EIGRP over DMVPN (dynamic tunnels):
A) Requires neighbor statement or discovery
B) Multicast may not work over tunnel
C) Unicast alternative config needed
D) All considerations

**Answer: D**

---

### Q56: Implement EIGRP fast reroute (FRR):
A) Pre-computed backup next-hop
B) Uses feasible successor
C) Sub-50ms rerouting possible
D) All features

**Answer: D**

---

### Q57: EIGRP metric manipulation for load balancing (unequal):
A) Adjust K-values (K1,K3)
B) Use variance multiplier
C) Configure per-neighbor weights
D) B is primary unequal mechanism

**Answer: D**

---

### Q58: EIGRP in complex multi-vendor environment:
A) Cisco-proprietary (not multi-vendor)
B) Some vendors support EIGRP now
C) Cisco focus typically
D) C most realistic enterprise view

**Answer: D**

---

### Q59: Design maintenance window EIGRP (no traffic disruption):
A) Graceful restart enabled
B) Stub configuration with delay
C) Pre-positioned alternates
D) All contribute

**Answer: D**

---

### Q60: Implement EIGRP auto-summary (legacy):
A) Summarizes at classful boundaries (RIPv2-like)
B) Disabled by default in modern IOS
C) Can cause routing blackholes if not careful
D) All true

**Answer: D**

---

### Q61: EIGRP query scope - preventing query storm:
A) Stub routers don't originate queries
B) Query paths limited by topology
C) Topology optimization reduces queries
D) All true

**Answer: D**

---

### Q62: Implement EIGRP in redundant links (mesh):
A) All paths considered
B) Feasible successor per destination
C) Without FS = active state/query
D) All mechanisms

**Answer: D**

---

### Q63: EIGRP with QoS (bandwidth-based routing):
A) Set interface bandwidth for metric
B) EIGRP uses this in calculation
C) Better paths via higher-speed links
D) All correct

**Answer: D**

---

### Q64: Design EIGRP as backup to primary OSPF:
A) Use redistribute with AD tuning
B) OSPF primary (AD 110), EIGRP backup (not redistributed)
C) Floating static as simplest option
D) All viable strategies

**Answer: D**

---

### Q65: EIGRP in hub-and-spoke non-broadcast (DMVPN):
A) Spoke-to-spoke communication requires hub transit
B) Summarization at hub limits overhead
C) Hub as router aggregator
D) All characterize hub-spoke

**Answer: D**

---

### Q66: Implement EIGRP multi-area (HQ-Branch):
A) Different AS numbers for areas (no)
B) Single AS with summarization
C) Stub routers at branches
D) B and C together

**Answer: D**

---

### Q67: EIGRP metric convergence in high-latency WAN:
A) Timers adjusted per link type
B) Hello interval higher for WAN
C) Hold time adjusted accordingly
D) All tuning needed

**Answer: D**

---

### Q68: Design disaster recovery (active-backup):
A) Primary routes via EIGRP
B) Backup routes via static/floating
C) EIGRP for primary network
D) All configure primary resilience

**Answer: D**

---

### Q69: EIGRP in virtualized environment (VRF):
A) Each VRF separate EIGRP instance
B) No cross-VRF route leakage
C) As number per VRF possible
D) All accurate

**Answer: D**

---

### Q70: Implement EIGRP prefix filtering (selectively advertise):
A) `distribute-list NAME out INTERFACE`
B) Blocks routes from being sent
C) Uses route-map for complex logic
D) All methods available

**Answer: D**

---

## COMMAND REFERENCE

```
! Enable EIGRP AS 100
router eigrp 100

! Configure network (wildcard mask)
network 10.0.0.0 0.255.255.255
network 172.16.0.0 0.0.255.255

! View EIGRP neighbors
show ip eigrp neighbors
show ip eigrp neighbors detail

! View EIGRP topology
show ip eigrp topology
show ip eigrp topology all-links

! View EIGRP routes
show ip route eigrp

! Configure hello interval
interface GigabitEthernet0/0
  hello-interval eigrp 100 10
  hold-time eigrp 100 30
exit

! Passive interface
passive-interface Serial0/0
passive-interface default

! Configure stub router
router eigrp 100
  eigrp stub connected summary
exit

! Configure EIGRP authentication
key chain EIGRP_KEYS
  key 1
    key-string MySecureKey123
  exit
exit

interface GigabitEthernet0/0
  ip authentication mode eigrp 100 md5
  ip authentication key-chain eigrp 100 EIGRP_KEYS
exit

! Configure variance (unequal-cost load-balancing)
router eigrp 100
  variance 2
exit

! Configure EIGRP metric K-values
router eigrp 100
  metric weights 0 1 0 1 0 0
exit

! Configure redistribution
redistribute static
redistribute rip

! Configure EIGRP summary address
interface Serial0/0
  ip summary-address eigrp 100 10.0.0.0 255.255.255.0
exit

! Configure offset-list
offset-list 1 in 5 Serial0/0

! View EIGRP configuration
show ip protocols
show running-config | section eigrp

! Enable graceful restart
router eigrp 100
  graceful-restart
exit

! Default route origination
router eigrp 100
  default-information originate
exit

! Clear EIGRP neighbor
clear ip eigrp neighbor 10.0.0.1

! Clear EIGRP topology
clear ip eigrp 100 topology

! Debug EIGRP
debug eigrp fsm
debug eigrp packets
debug ip eigrp neighbor
undebug all
```

---

## KEY CONCEPTS

1. **DUAL (Diffusing Update Algorithm)**: Loop-free alternative paths ensuring convergence
2. **Successor**: Best route to destination
3. **Feasible Successor**: Backup route with advertised distance < feasible distance
4. **Active State**: Querying neighbors when successor unavailable
5. **Passive State**: Stable state with known route
6. **Administrative Distance**: 90 (internal), 170 (external, redistributed)
7. **Metric Components**: K1 (bandwidth), K2 (load), K3 (delay), K4 (reliability), K5 (MTU) - default K1=1, K3=1, others=0
8. **Feasibility Condition**: Ensures loop-free paths
9. **Query/Reply**: EIGRP messages for active/passive transitions
10. **Stub Router**: Reduces queries, typically for branch/leaf nodes
11. **Summarization**: Manual aggregation of multiple routes
12. **Variance**: Unequal-cost load-balancing multiplier
13. **Graceful Restart**: Preserves neighbor state during reload
14. **IPv6 EIGRP**: Separate protocol configuration alongside IPv4
15. **Named Mode**: Modern EIGRP configuration allowing multiple protocols in one config

