# Static Routing MCQ Quiz

---

## EASY LEVEL

### Q1: What is Static Routing?
A) Routes manually configured by administrator
B) Routes learned automatically from neighbors
C) Routes based on network topology
D) Routes that change with time

**Answer: A**

---

### Q2: In Cisco, which command configures a static route?
A) `route 192.168.1.0`
B) `ip route 192.168.1.0 255.255.255.0 192.168.0.1`
C) `static route 192.168.1.0`
D) `configure static 192.168.1.0`

**Answer: B**

---

### Q3: A default route destination address is:
A) 192.168.0.0
B) 0.0.0.0
C) 255.255.255.255
D) Network-specific

**Answer: B**

---

### Q4: Syntax: `ip route 10.0.0.0 255.255.255.0 192.168.1.1`. What is 192.168.1.1?
A) Destination network
B) Next hop (gateway)
C) Subnet mask
D) Interface name

**Answer: B**

---

### Q5: What is the administrative distance of static route by default?
A) 0
B) 1
C) 10
D) 120

**Answer: B**

---

### Q6: Static route with administrative distance 200: is it preferred over RIP (120)?
A) Yes, always preferred
B) No, RIP is preferred
C) Depends on topology
D) They cannot coexist

**Answer: B**

---

### Q7: Cannot reach static route destination. What to check first?
A) Ensure next-hop interface is up
B) Ensure there's a route back (return path)
C) Both A and B
D) Check CPU usage

**Answer: C**

---

### Q8: Configure static route via interface (instead of next-hop IP):
A) `ip route 10.0.0.0 255.255.255.0 FastEthernet0/0`
B) `ip route 10.0.0.0 255.255.255.0 via FastEthernet0/0`
C) Not possible - must use IP
D) `route via interface FastEthernet0/0`

**Answer: A**

---

### Q9: Static route with metric/cost:
A) `ip route 10.0.0.0 255.255.255.0 192.168.1.1 cost 5`
B) `ip route 10.0.0.0 255.255.255.0 192.168.1.1 5`
C) Metric automatic
D) Not used in static routing

**Answer: B**

---

### Q10: View all configured static routes:
A) `show routes static`
B) `show ip route static`
C) `show static routes`
D) `show routing static`

**Answer: B**

---

### Q11: Remove a static route:
A) `delete ip route 10.0.0.0 255.255.255.0 192.168.1.1`
B) `no ip route 10.0.0.0 255.255.255.0 192.168.1.1`
C) `remove route`
D) `clear static route`

**Answer: B**

---

### Q12: Default route typically points to:
A) Internal network
B) Local subnet
C) Internet gateway / ISP router
D) Loopback interface

**Answer: C**

---

### Q13: Configure default route to 192.168.0.1:
A) `ip route 0.0.0.0 0.0.0.0 192.168.0.1`
B) `ip default-route 192.168.0.1`
C) `ip route default 192.168.0.1`
D) Only A is correct

**Answer: A**

---

### Q14: What happens with multiple static routes to same destination?
A) First configured used
B) Last configured used
C) All used (load balancing)
D) Error generated

**Answer: C** (if equal metric/AD)

---

### Q15: Static route uses less CPU than dynamic routing protocols?
A) Yes
B) No
C) Same CPU usage
D) Depends on interval

**Answer: A**

---

### Q16: Static routes are displayed in routing table with which code?
A) D (EIGRP)
B) O (OSPF)
C) S (Static)
D) R (RIP)

**Answer: C**

---

### Q17: Configure recursive next-hop static route:
A) Not possible - must be direct next-hop
B) Possible - router resolves via its routing table
C) Requires static route to next-hop router
D) Both B and typically C for best practice

**Answer: D**

---

### Q18: Static route with administrative distance 50:
A) `ip route 10.0.0.0 255.255.255.0 192.168.1.1 50`
B) `ip route 10.0.0.0 255.255.255.0 192.168.1.1 administrative-distance 50`
C) Not possible
D) `static-route ad 50`

**Answer: A**

---

### Q19: Floating static route - backup route with higher AD:
A) Not supported
B) Supported - appears in table only if primary down
C) Always active
D) Requires OPSF

**Answer: B**

---

### Q20: Remove all static routes:
A) `no ip route *`
B) `clear static routes`
C) Remove individually with `no ip route`
D) `restart routing`

**Answer: C**

---

## MEDIUM LEVEL

### Q21: Configure static route to 172.16.0.0/16 via next-hop 10.0.0.1 with AD 200:
A) `ip route 172.16.0.0 255.255.0.0 10.0.0.1 200`
B) `ip route 172.16.0.0 255.255.0.0 10.0.0.1 ad 200`
C) Same as A (10 is seconds/metric, 200 is AD... depends on version)
D) Not possible in one command

**Answer: A**

---

### Q22: Static route via interface - when used?
A) For point-to-point links
B) For serial WAN links
C) For Ethernet links
D) A and B only

**Answer: D** (Typically point-to-point where next-hop is obvious)

---

### Q23: Create floating static route: primary (AD 1), backup (AD 200) to 192.168.0.0/24:
A) Create one route with AD 1, then one with AD 200
B) Both routes in config, router automatically switches
C) Requires manual configuration change
D) Not automatically failover

**Answer: B**

---

### Q24: Static route next-hop must be:
A) Directly connected to source router
B) Reachable via existing routing table
C) Both possible
D) Only directly connected

**Answer: C**

---

### Q25: Configure static route to 10.1.0.0/24 with equal-cost redundancy (two paths):
A) `ip route 10.1.0.0 255.255.255.0 192.168.1.1`
B) `ip route 10.1.0.0 255.255.255.0 192.168.1.1`
C) `ip route 10.1.0.0 255.255.255.0 192.168.1.2`
D) Multiple of these separately create load-balancing

**Answer: D**

---

### Q26: View static route details including next-hop and AD:
A) `show ip route 10.0.0.0`
B) `show ip route static 10.0.0.0`
C) `show ip route | include Static`
D) All show similar info

**Answer: D**

---

### Q27: Static route to 192.168.1.0/24 via Serial0/0 interface - when is next-hop needed?
A) Always needed
B) Not needed for point-to-point links
C) Optional - can use interface instead
D) Only for Ethernet

**Answer: B**

---

### Q28: Recursive lookup of static route:
A) Route points to another route
B) Table resolves via multiple lookups
C) Can cause routing loop if misconfigured
D) All of above

**Answer: D**

---

### Q29: Static route with track object (for failover):
A) `ip route 10.0.0.0 255.255.255.0 192.168.1.1 track 1`
B) Requires object tracking first: `track 1 ...`
C) Both A and B
D) Not supported

**Answer: C**

---

### Q30: Summarize subnets 10.1.0.0/24, 10.2.0.0/24, 10.3.0.0/24 into one static route:
A) Create three separate routes
B) Single static route to 10.0.0.0/22 (if only these three)
C) Use 10.0.0.0/8 with longer prefix for more
D) Depends on exact subnets

**Answer: D** (10.1, 10.2, 10.3 are separate - can't summarize easily)

---

### Q31: Static route to 0.0.0.0/0 (default) created, why would you use it?
A) For networks without internet access
B) All unknown destinations go to this route
C) Fallback route for unmatched traffic
D) All of above plus Internet gateway

**Answer: D**

---

### Q32: Configure static route with name/description:
A) `ip route 10.0.0.0 255.255.255.0 192.168.1.1 name "TO_HQ"`
B) Create route then use `description` command (no such command)
C) Refer by metrics only
D) Names not supported

**Answer: D** (No built-in naming for static routes)

---

### Q33: Static route propagation via routing protocol:
A) Automatic distribution
B) Manual redistribution required
C) Uses default redistribution commands
D) Not possible

**Answer: B**

---

### Q34: Effect of deleting next-hop interface on active static route:
A) Route automatically removed
B) Route remains but unusable
C) Router tries alternate next-hop
D) Link remains cached

**Answer: B**

---

### Q35: Multiple static routes same destination, different AD - which is active?
A) All active
B) Lowest AD only
C) Highest AD only
D) User configured

**Answer: B**

---

### Q36: Permanent static route across reboots:
A) Automatically saved
B) Must be in startup-config
C) Requires explicit save
D) Commands needed?

**Answer: B** (Must save with `copy running-config startup-config`)

---

### Q37: Static route with mask 255.255.255.255 (/32) - what is this?
A) Host route to single IP
B) Network route
C) Broadcast route
D) Not valid

**Answer: A**

---

### Q38: Create three equal-cost static paths to 10.0.0.0/24 for load-balancing:
A) Three identical `ip route` commands with different next-hops
B) Use EqualCost parameter
C) Cisco does this automatically per-destination
D) Requires multipath command

**Answer: A**

---

### Q39: Next-hop address that doesn't exist what happens?
A) Route becomes inactive (kernel rejects)
B) Route appears in table (if no other validation)
C) Depends on resolver setting
D) Route causes error

**Answer: A** (in modern IOS with better validation)

---

### Q40: Static route via 192.168.0.5 when interface shows 192.168.0.0/24 - valid?
A) Yes - it's in subnet
B) No - cannot route out interface it's on
C) Valid but unusual
D) Requires explicit permission

**Answer: A**

---

## HARD LEVEL

### Q41: Implement floating static route where primary is OSPF, backup is static with AD 250:
A) Create primary OSPF naturally, add static route AD 250
B) Primary is via ip route AD 110, add static AD 250
C) Requires redistribution first
D) Automatic fail-over is guaranteed

**Answer: A** (OSPF AD is 110, static primary usually AD 1 or less, backup static AD 250)

---

### Q42: Configure static route with object tracking for interface (if up, use route):
A) Command: `ip route ... track 1` after creating track object
B) `track 1 interface GigabitEthernet0/0 line-protocol`
C) Both A and B required
D) Cisco doesn't support this

**Answer: C**

---

### Q43: Recursive static route to 10.0.0.0/24 via next-hop 172.16.0.1 (itself learned via static to 172.16.0.0/24). Validate this works:
A) Yes - recursive lookups supported
B) No - creates simulation infinite loop
C) Yes but extra lookup overhead
D) Depends on IOS version

**Answer: A**

---

### Q44: Static route redistribution into OSPF - what command enables it?
A) `redistribute static into ospf`
B) `redistribute static subnets` (inside OSPF config)
C) Automatic if using OSPF
D) Not supported

**Answer: B**

---

### Q45: Configure high-availability static routing with two routes, load-balance traffic (round-robin):
A) Two identical routes different next-hops = automatic per-destination load-balancing
B) Requires CEF/FIB enabling
C) Both paths used simultaneously
D) A and B ensure active-active

**Answer: D**

---

### Q46: Static route to Null0 interface - purpose:
A) Routes packet to null (dropped)
B) Used as discard route / blackhole
C) Prevent routing loop
D) All of above

**Answer: D**

---

### Q47: Summarize routes into supernet for static routing - when used?
A) On edge router pointing to core
B) Reduce routing table size
C) Aggregation point to Internet
D) All of above scenarios

**Answer: D**

---

### Q48: Static route with Cisco ASA - same syntax as IOS?
A) Yes - identical
B) Mostly same, some differences in commands
C) Different syntax
D) Not supported on ASA

**Answer: B**

---

### Q49: Configure default static route in a VRF context:
A) Same global command works
B) `ip route vrf NAME 0.0.0.0 0.0.0.0 ...`
C) Separate from global routing table
D) Both B and C

**Answer: D**

---

### Q50: Static route conflict with connected route same destination - which wins?
A) Static route preferred
B) Connected route preferred
C) Error/warning generated
D) Manual priority setting

**Answer: B**

---

### Q51: When does static route Administrative Distance become critical?
A) Always important
B) When multiple paths exist to same destination
C) Determines best path if AD differs
D) B and C - critical for path selection

**Answer: D**

---

### Q52: Remove static route without knowing exact next-hop:
A) `no ip route 10.0.0.0 255.255.255.0` (without next-hop)
B) Must specify exact match including next-hop
C) View first then remove
D) Unknown next-hop removal not possible

**Answer: B**

---

### Q53: Static routes in redundancy scenario (Active-Standby) - what's needed?
A) Primary AD=1, Standby AD=200
B) Automatic failover via HSRP/VRRP
C) Static routes on both, separate designs
D) Single shared static config

**Answer: A**

---

### Q54: Impact of static routing on network scalability:
A) Scalable - no protocol overhead
B) Not scalable - manual config burden
C) Scales well with network growth
D) Depends on network size

**Answer: B**

---

### Q55: Static route via recursive next-hop 192.168.1.5 when no direct route to that IP:
A) Route appears but inactive
B) Automatic activation when next-hop reachable
C) Error generated
D) Route assumes existence

**Answer: A**

---

### Q56: Default route static with preference to dynamic route - how?
A) Default static AD higher than any dynamic
B) Default route AD 254 (or higher), dynamic protocol default
C) Enable default route in protocol
D) Manual priority in routing table

**Answer: A**

---

### Q57: Static route with next-hop on different subnet - must ensure:
A) IP is reachable via existing routing table
B) Interface to that subnet is up
C) No static loop back
D) All requirements

**Answer: D**

---

### Q58: Convert dynamic routing network to static - benefit?
A) No more protocol bandwidth
B) Reduce CPU usage
C) Fixed routing regardless of topology
D) A and B are benefits

**Answer: D**

---

### Q59: Static route per-pixel load balancing (different paths per destination IP):
A) Automatic with CEF in modern IOS
B) Manual per-route configuration
C) Requires specific load-balance command
D) Not possible

**Answer: A**

---

### Q60: Design static routing for stub network (dead-end branch):
A) One static route out via default route
B) Multiple static routes not needed
C) Static route to summary supernet
D) All apply per scenario

**Answer: D**

---

### Q61: Static route pointing to next-hop that is itself learned via static route:
A) Not possible - creates loop prevention
B) Possible if distinct networks (recursive)
C) Requires explicit loop check command
D) IOS automatically creates virtual loop

**Answer: B**

---

### Q62: Implement multipath static routing with unequal-cost load-balancing:
A) Not possible - only equal-cost
B) Different AD routes (with tracking objects)
C) Cisco CEF allows unequal metrics
D) Requires custom routing policy

**Answer: B**

---

### Q63: Static route during failover from ISP A to ISP B:
A) Manual re-configuration needed
B) Floating static route with AD
C) Automatic failover in static config
D) Both B (automatic) and tracking

**Answer: D**

---

### Q64: Large enterprise with 100+ subnets - static routing practical?
A) Yes - manageable
B) No - requires dynamic routing
C) Possible but error-prone
D) Depends on topology stability

**Answer: D**

---

### Q65: Static route to multi-hop next-hop (IP is 3 hops away) - works?
A) No - must be directly connected
B) Yes - router resolves recursively
C) Possible if route exists in table
D) Depends on recursive-resolver depth

**Answer: B**

---

### Q66: Configure ECMP (Equal-Cost Multi-Path) with static routes:
A) Automatic if routes have equal AD
B) Requires explicit CEF/FIB setup
C) Both routes must have identical parameters
D) A most accurate for equal-cost load-balance

**Answer: A**

---

### Q67: Static route with administrative distance 0 - what does this mean?
A) Most preferred route
B) Connected route level (can't override)
C) Equivalent to directly connected
D) Least preferred

**Answer: C**

---

### Q68: Implement static routing for backup internet link (load-balance across primary MPLS):
A) MPLS static (AD 50), Internet static (AD 150)
B) Both active - CEF load-balances
C) Internet preferred only if primary down
D) Dynamic routing better here

**Answer: A**

---

### Q69: Static route to entire AS via BGP peer - which takes precedence?
A) Static (lower AD usually)
B) BGP if specific enough
C) Depends on prefix length / specificity
D) Manual selection needed

**Answer: C**

---

### Q70: Summarize static routes in hub-and-spoke topology:
A) Hub aggregates all spokes into one summary
B) Each spoke advertises itself
C) Central switch distributes summary
D) Each spoke needs specific routes

**Answer: A**

---

## COMMAND REFERENCE

Common Static Routing Commands:
```
! Configure static route to destination via next-hop
ip route 10.0.0.0 255.255.255.0 192.168.1.1

! Configure static route via interface
ip route 10.0.0.0 255.255.255.0 Serial0/0

! Configure with administrative distance
ip route 10.0.0.0 255.255.255.0 192.168.1.1 200

! Configure default route
ip route 0.0.0.0 0.0.0.0 192.168.0.1

! View all static routes
show ip route static
show ip route | include S

! View specific route
show ip route 10.0.0.0

! View routing table with details
show ip route

! Remove static route
no ip route 10.0.0.0 255.255.255.0 192.168.1.1

! Floating static route (backup)
ip route 10.0.0.0 255.255.255.0 192.168.1.1 1     ! Primary
ip route 10.0.0.0 255.255.255.0 192.168.1.2 200   ! Backup

! Static route with tracking object
ip route 10.0.0.0 255.255.255.0 192.168.1.1 track 1

! Create tracking object for interface
track 1 interface GigabitEthernet0/0 line-protocol

! Static blackhole route (discard)
ip route 10.0.0.0 255.255.255.0 Null0 250

! Redistribute static routes into OSPF
router ospf 1
  redistribute static subnets
exit

! Equal-cost load-balancing (multiple routes same metrics)
ip route 10.0.0.0 255.255.255.0 192.168.1.1
ip route 10.0.0.0 255.255.255.0 192.168.1.2
ip route 10.0.0.0 255.255.255.0 192.168.1.3

! Save configuration
copy running-config startup-config
write memory

! Debug static routing
debug ip routing
debug ip route tracking
undebug all

! View policy-based route
show route-map
show ip policy
```

---

## KEY CONCEPTS

1. **Static Route**: Manually configured, doesn't change unless admin changes it
2. **Default Route**: Catch-all route (0.0.0.0/0) for unknown destinations
3. **Next-Hop**: Gateway through which traffic is routed
4. **Administrative Distance (AD)**: Route preference metric (lower = preferred)
5. **Floating Route**: Backup static with higher AD, activates if primary down
6. **Recursive Lookup**: Router resolves next-hop via existing routing table
7. **Connected Route**: Directly connected network (lowest AD automatically)
8. **Route Aggregation**: Summarizing multiple routes into supernet
9. **Null0 Interface**: Black-hole route that discards traffic
10. **Equal-Cost Load-Balancing**: Multiple paths with same metrics share traffic
11. **Track Object**: Monitoring (interface, IP, path) to remove route if condition fails
12. **VRF Routing**: Separate routing tables per VRF context
13. **Redistribution**: Sharing static routes with dynamic protocols
14. **Route Poisoning**: Preventing loop with discard route
15. **Point-to-Point**: Often uses /30 or /31 with next-hop as other end

