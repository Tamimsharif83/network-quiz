# RIP (Routing Information Protocol) MCQ Quiz

---

## EASY LEVEL

### Q1: What does RIP stand for?
A) Routing Information Protocol
B) Route Information Process
C) Rapid Internet Protocol
D) Remote IP Protocol

**Answer: A**

---

### Q2: RIPv1 uses which routing algorithm?
A) Dijkstra's algorithm
B) Bellman-Ford algorithm
C) Floyd-Warshall algorithm
D) Greedy algorithm

**Answer: B**

---

### Q3: Default administrative distance for RIPv1/RIPv2?
A) 90
B) 100
C) 110
D) 120

**Answer: D**

---

### Q4: Maximum hop count in RIP?
A) 15
B) 16
C) 30
D) Unlimited

**Answer: A**

---

### Q5: Enable RIP on router - first command?
A) `enable rip`
B) `router rip`
C) `rip enable`
D) `configure rip`

**Answer: B**

---

### Q6: RIP version specification command?
A) `version rip 2`
B) `version 2`
C) `rip version 2`
D) `set version 2`

**Answer: B**

---

### Q7: Configure network 192.168.1.0 in RIP:
A) `network 192.168.1.0`
B) `network 192.168.1.0 255.255.255.0`
C) `configure network 192.168.1.0`
D) `add network 192.168.1.0`

**Answer: A**

---

### Q8: RIPv1 sends updates as:
A) Unicast
B) Multicast 224.0.0.9
C) Broadcast 255.255.255.255
D) Both B and C

**Answer: C**

---

### Q9: RIPv2 sends updates as:
A) Unicast only
B) Multicast 224.0.0.9
C) Broadcast
D) Direct to neighbor

**Answer: B**

---

### Q10: RIP update interval (default)?
A) 10 seconds
B) 20 seconds
C) 30 seconds
D) 60 seconds

**Answer: C**

---

### Q11: RIP invalid timer (route marked invalid after):
A) 60 seconds
B) 90 seconds
C) 120 seconds
D) 180 seconds

**Answer: D**

---

### Q12: View RIP status and neighbors:
A) `show rip status`
B) `show ip rip protocol`
C) `show ip protocols`
D) `show routing protocols`

**Answer: C**

---

### Q13: What is RIP holdown timer?
A) Waits for update confirming better route
B) Ignores worse routes for this time
C) Time to wait for route confirmation
D) All of above

**Answer: D**

---

### Q14: RIPv1 vs RIPv2 - what's a key difference?
A) RIPv2 uses multicast (224.0.0.9)
B) RIPv2 supports subnetting/CIDR
C) RIPv2 supports authentication
D) All of above

**Answer: D**

---

### Q15: RIP triggers update when:
A) Route changes
B) Regular 30-second interval
C) Both
D) Manual command

**Answer: C**

---

### Q16: Remove network from RIP:
A) `no network 192.168.1.0`
B) `remove network 192.168.1.0`
C) `delete network 192.168.1.0`
D) Not possible

**Answer: A**

---

### Q17: Split horizon prevents:
A) Routing loops
B) Counting to infinity
C) Sending route back to source
D) All of above

**Answer: C**

---

### Q18: Passive interface in RIP:
A) Interface receives updates only
B) Interface sends updates only
C) Interface disabled
D) Backup interface

**Answer: A**

---

### Q19: Disable RIP on all interfaces:
A) `passive-interface default`
B) `no network all`
C) `shutdown rip`
D) `disable interface`

**Answer: A**

---

### Q20: RIP metric is based on:
A) Bandwidth
B) Delay
C) Hop count
D) Cost

**Answer: C**

---

## MEDIUM LEVEL

### Q21: Configure RIPv2 with authentication (MD5):
A) In RIP interface context, just enable MD5
B) Configure key-chain, then apply to interface
C) Use `authentication md5` on interface
D) RIP doesn't support authentication

**Answer: B**

---

### Q22: RIP sends update with hop count 16 - what happens?
A) Some routers accept it
B) Route is unreachable (not advertised)
C) Converted to 15 hops
D) Update rejected

**Answer: B**

---

### Q23: Configure offset-list to increase RIP metric from neighbor by 5:
A) `offset-list IN 5 192.168.1.1`
B) `offset-list 0 in 5 192.168.1.1`
C) At RIP level: `offset-list 0 in 5`
D) Not possible

**Answer: B**

---

### Q24: RIP interface delay/timing tuning:
A) `timers basic update invalid holddown`
B) Example: `timers basic 10 180 180`
C) Changes global RIP timing
D) Both A and B

**Answer: D**

---

### Q25: Redistribute static routes into RIP:
A) `redistribute static`
B) Inside RIP router config: `redistribute static`
C) Both valid
D) Not supported

**Answer: B**

---

### Q26: RIP neighbor lists maximum size:
A) 6 routers
B) 15 routers
C) 30 routers
D) Unlimited

**Answer: D**

---

### Q27: View RIP neighbors:
A) `show ip rip neighbors`
B) `show rip neighbors`
C) `show protocols neighbors`
D) `show ip protocols` (shows interfaces)

**Answer: D**

---

### Q28: RIP database / routing table entry learning:
A) All routers must know all networks
B) Router only needs routes from direct neighbors
C) Central database maintained
D) Each router has partial topology

**Answer: B**

---

### Q29: RIP route preference between tied (same AD) routes:
A) First learned used
B) Load balance across both
C) Manual priority
D) Latest received used

**Answer: B**

---

### Q30: Poison reverse - what is it?
A) Advertising unreachable routes (metric 16)
B) Preventing loop by splitting horizon
C) Rejecting bad routes
D) Route authentication

**Answer: A**

---

### Q31: Configure RIP conditional advertisement (route filter):
A) `distribute-list in/out`
B) `route-map` based filtering
C) `access-list` referencing
D) All methods available

**Answer: D**

---

### Q32: RIPv2 with subnet information - what's new?
A) Carries subnet masks in updates
B) CIDR support
C) Classless routing
D) All of above

**Answer: D**

---

### Q33: RIP silent interface - packets sent but not received:
A) `passive-interface except` approach (no)
B) No such feature - passive is listen-only
C) Use `quiet interface`
D) Not needed

**Answer: B**

---

### Q34: How many routes fit in single RIP packet?
A) 25
B) 156
C) 255
D) Unlimited

**Answer: A** (limited by packet size)

---

### Q35: RIP convergence time for network with 15 hops:
A) < 1 minute
B) 5 minutes
C) 10 minutes
D) 15+ minutes

**Answer: D**

---

### Q36: Default RIP weight metric per hop:
A) 1
B) 5
C) 10
D) 16

**Answer: A**

---

### Q37: RIPv2 supernet aggregation:
A) Automatic aggregation at boundary
B) Manual configuration required
C) No aggregation
D) Per-interface setting

**Answer: A**

---

### Q38: Disable RIP on specific interface:
A) `passive-interface` is approach
B) Configure `network` excluding this interface
C) Both work
D) Interface removal

**Answer: C**

---

### Q39: RIP backup route via neighbor (similar cost):
A) Not supported - deterministic path
B) Uses both for load-balance
C) Explicit configuration
D) Needs cost adjustment

**Answer: B**

---

### Q40: RIP maximum packet size:
A) 512 bytes
B) 1024 bytes
C) MTU-dependent
D) 1500 bytes

**Answer: A**

---

## HARD LEVEL

### Q41: Implement RIPv2 with authentication and distribution list:
A) Configure key-chain, apply to interface, and distribute-list in/out
B) Requires route-map for filtering
C) Both methods can co-exist
D) Prioritize distribute-list

**Answer: A** (standard approach: auth + filtering)

---

### Q42: RIP database inconsistency when network partitions - recovery time?
A) Immediate
B) Invalid timer (180 seconds)
C) Flush timer (240 seconds)
D) Depends on reconvergence

**Answer: C**

---

### Q43: RIPv1 classful addressing - what's the implication?
A) Only /8, /16, /24 networks
B) No VLSM support
C) Cannot mix different masks
D) All of above

**Answer: D**

---

### Q44: Configure RIP to only send updates (not receive):
A) Not possible - RIP requires bidirectional updates
B) Turn off network command, enable passive-interface, then redistribute
C) Not a valid configuration
D) Requires custom filtering

**Answer: C**

---

### Q45: RIP with EIGRP/OSPF redistribution - AD implications?
A) RIP (120) likely overridden if EIGRP (90) exists
B) Redistribution changes AD
C) Needs AD tuning to ensure preference
D) All of above

**Answer: D**

---

### Q46: Prevent RIP from advertising specific network (without passive-interface):
A) `network` command selective
B) Use `distribute-list` with access-list
C) Use `route-map` with deny
D) B or C

**Answer: D**

---

### Q47: RIP unequal-cost load balancing:
A) Not possible
B) Possible via variance (EIGRP-like)
C) Manual metric adjustment
D) Not in RIP standard

**Answer: D**

---

### Q48: Implement RIP for stub area (branch) to corporate core:
A) Configure RIP at both ends
B) Consider static default route
C) RIP default-route advertisement useful
D) Dynamic RIP across branch links

**Answer: C**

---

### Q49: RIP triggered updates vs periodic:
A) Both can occur
B) Triggered only on change
C) Periodic always 30 seconds
D) Triggered within 5 seconds

**Answer: A** (periodic + triggered on change)

---

### Q50: Counting to infinity in RIP - Bellman-Ford mitigation:
A) Maximum hopcount 15
B) Split horizon
C) Poison reverse
D) All three combined

**Answer: D**

---

### Q51: RIPv2 multicast 224.0.0.9 - advantage over broadcast?
A) Reduced network load
B) Only RIP routers process
C) Better for security
D) All of above

**Answer: D**

---

### Q52: Enterprise migration from RIPv2 to OSPF - strategy?
A) Pure cutover (stop one, start other)
B) Redistribute for parallel-run period
C) Static routes during transition
D) B or C depend on plan

**Answer: D**

---

### Q53: Design RIP network with 3 hops max for convergence:
A) Feasible - updates take ~90 seconds
B) Feasible - triggered updates faster
C) Impractical for production
D) Depends on update interval tuning

**Answer: B**

---

### Q54: RIP metric artificially increased via offset-list:
A) Deprefers route but keeps valid
B) Useful for traffic engineering
C) Both true
D) No benefit

**Answer: C**

---

### Q55: Reserved bit field (RIPv2) - what is it?
A) Future use
B) Currently unused
C) Must be zero in RFCs
D) All correct

**Answer: D**

---

### Q56: RIP graceful shutdown (no black-hole):
A) Set metrics to 16 gradually
B) Send poison reverse to neighbors
C) Generate triggered updates
D) B or C or combination

**Answer: D**

---

### Q57: Debugging RIP receives vs sends:
A) `debug ip rip packet`
B) `debug ip rip db`
C) Both show different info
D) Single debug shows both

**Answer: C**

---

### Q58: RIP subinterface routing:
A) Same as physical interface
B) VLAN subinterface fully supported
C) Each subinterface separate RIP instance
D) A and B

**Answer: D**

---

### Q59: RIP convergence with flapping link:
A) Rapid convergence
B) Bouncing prevents convergence
C) Hold-down timer prevents oscillation
D) Manual intervention needed

**Answer: C**

---

### Q60: Design hybrid RIP+static routing for high-availability:
A) RIP for dynamic edges, static for core
B) Static on primary, RIPv2 backup
C) Depends on topology
D) Impractical - avoid mixing

**Answer: C**

---

### Q61: RIP transaction authentication code (TAC):
A) MD5 hash of message
B) Simple password hash
C) Better than plain-text
D) Both A and C

**Answer: D**

---

### Q62: RIPv2 next-hop improvement - what is it?
A) Specifies next-hop in update
B) Reduces routing table size
C) Improves convergence
D) Prevents sub-optimal routes

**Answer: D**

---

### Q63: Originate default route via RIP:
A) `default-information originate`
B) `network 0.0.0.0`
C) Applicable to other protocols more
D) Both A and B

**Answer: A**

---

### Q64: RIP with interface enable/disable (bringing down interface):
A) Immediately invalidates routes
B) Invalid timer applies
C) Neighbor detects after timeout
D) Network reconverges per timers

**Answer: D**

---

### Q65: RIP summarization (aggregate subnets into fewer):
A) Automatic at network boundary
B) Manual per configuration
C) RIPv2 only
D) Improves scalability

**Answer: C** (RIPv2 with auto-summary off)

---

### Q66: Configure multiple RIP instances on same router:
A) Not possible - one global RIP
B) Separate AS numbers allowed
C) Via VRF instances
D) C primarily, or separate VRFs

**Answer: C**

---

### Q67: Performance impact of RIPv2 authentication on network:
A) Minimal - modern hardware
B) Marginal increase in CPU
C) Slight delay per update
D) All minimal in modern routers

**Answer: D**

---

### Q68: RIP performance in LAN-to-LAN steady-state:
A) Converges once, stable
B) Periodic updates only (no changes)
C) Minimal CPU after convergence
D) All accurate

**Answer: D**

---

### Q69: RIP next-hop field in RIPv2 update - when used?
A) When next-hop is not sending router
B) For suboptimal routing elimination
C) Improves aggregate path selection
D) All of above

**Answer: D**

---

### Q70: Migration path: RIPv1 → RIPv2 → OSPF?
A) Direct RIPv2 to OSPF better
B) Gradual via RIPv2 as intermediate
C) Completely different protocols
D) RIPv1 can coexist with OSPF partly

**Answer: B**

---

## COMMAND REFERENCE

```
! Enable RIP routing
router rip

! Configure RIP version
version 2

! Enable RIP on network
network 192.168.0.0
network 10.0.0.0

! Exit RIP config
exit

! View RIP protocol debug
show ip protocols

! View RIP routes in routing table
show ip route rip

! Debug RIP packet details
debug ip rip packet

! Configure passive interface (receive only)
passive-interface FastEthernet0/0

! Make all passive, except specified
passive-interface default
no passive-interface Serial0/0

! Configure RIP timers
timers basic 10 180 180 240

! Enable RIPv2 authentication (key-chain)
key chain RIP_KEYS
  key 1
    key-string mypassword123
  exit
exit

! Apply authentication on interface
interface FastEthernet0/0
  ip rip authentication mode md5
  ip rip authentication key-chain RIP_KEYS
exit

! Redistribute static routes
redistribute static

! Filter outgoing RIP routes
distribute-list 1 out FastEthernet0/0

! Filter incoming RIP routes
distribute-list 1 in FastEthernet0/0

! Send default route
default-information originate

! Clear RIP database
clear ip rip database
```

---

## KEY CONCEPTS

1. **RIPv1 vs RIPv2**: v1 classful, v2 classless; v2 uses multicast (224.0.0.9)
2. **Maximum Hop Count**: 15 (16 = unreachable)
3. **Administrative Distance**: 120 (lowest for dynamic protocols before static/connected)
4. **Metric**: Hop count (each router = +1)
5. **Update Interval**: 30 seconds (periodic)
6. **Invalid Timer**: 180 seconds (after no update, mark unreachable)
7. **Flush Timer**: 240 seconds (remove route completely)
8. **Hold-Down Timer**: 180 seconds (ignore worse routes)
9. **Split Horizon**: Don't send route back to source interface
10. **Poison Reverse**: Send metric 16 for unreachable routes
11. **Triggered Update**: Immediate update on topology change
12. **Passive Interface**: Receive updates, don't send
13. **Authentication**: MD5 in RIPv2 (simple in v1)
14. **Convergence**: Slow (up to ~3-5 minutes for 15 hops)
15. **Scalability**: Limited (max 15 hops = max network diameter)

